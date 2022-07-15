Gickup
=========

Installs [gickup](https://github.com/cooperspencer/gickup) as a docker container.


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
gickup_container_user: pi
```
user running the container 

```
gickup_timezone: "Europe/Madrid"
```
timezone for cron job

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

