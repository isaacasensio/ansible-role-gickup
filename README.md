Gickup
=========

Installs [gickup](https://github.com/cooperspencer/gickup) docker container as a daemon.


Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

```
gickup_image: "buddyspencer/gickup:latest"
```
The version of the docker image to run as a container.

```
gickup_host_path: /etc/gickup
```
Host path which stores Gickup configuration.

```
gickup_host_backup_path: /var/backup
```
Host path where all backups will be stored.

```
gickup_container_user: gickup
```
user running the container

```
gickup_timezone: "Europe/Madrid"
```
timezone for cron job

```
gickup_config_content: |
source:
  github:
    - token: some-token
      user: some-user  
```
Gickup configuration. More info here: https://github.com/cooperspencer/gickup/blob/main/conf.example.yml

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - iasensio.gickup

License
-------

MIT

