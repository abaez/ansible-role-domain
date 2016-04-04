Docker
=========
[![license][2i]][2p]
[![twitter][5i]][5p]

A nginx reverse proxy based on docker.

Description
-----------

A role to use nginx reverse proxy docker container for use for sub domains or domains of your site/app. You can learn more about the [container here][4].

Role Variables
--------------

There is one variable that needs to be changed. That's the `user.name` variable. You can find this variable in **vars/main.yml**. Change the variable to the user that you want to manage the docker container through systemd.

Requirements
------------

Need to have docker already installed one way or another. You can use the handy dandy [docker role][3] I have for the task.

Usage
-----

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

``` yaml
- hosts: servers
    roles:
        - docker
        - domain
```

Author Information
------------------

[Alejandro Baez][1]

[1]: https://keybase.io/baez
[2i]: https://img.shields.io/badge/license-BSD_2-green.svg
[2p]: ./LICENSE
[3]: https://galaxy.ansible.com/abaez/docker/
[4]: https://hub.docker.com/r/jwilder/nginx-proxy/
[5i]: https://img.shields.io/badge/twitter-a_baez-blue.svg
[5p]: https://twitter.com/a_baez
