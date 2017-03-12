ansible-role-laraveldeploy
=========
[![Build Status](https://travis-ci.org/benlipp/ansible-role-laraveldeploy.svg?branch=master)](https://travis-ci.org/benlipp/ansible-role-laraveldeploy)


An ansible role to deploy a Laravel app.

Requirements
------------

See the Dependencies section

Role Variables
--------------

- `repo`: an HTTPS clone URL of the repo you wish to deploy
- `destination`: where the app should be deployed on the server

Dependencies
------------
    - geerlingguy.composer
    - geerlingguy.git

Example Playbook
----------------

    - hosts: webservers
      roles:
        - role: benlipp.laraveldeploy
            repo: "https://github.com/benlipp/ansible-role-laraveldeploy.git"
            destination: /srv/www/laravel-app

License
-------

MIT
