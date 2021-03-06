LVM-ROCA-prototype
==================

Meta-repository to start lvm roca-prototype in a automated, dockerized environment.  

**!This project was rebranded. The most recent version can be found [here as crimson assurance](https://github.com/crimson-assurance).**

Prerequisites
--------------

* make sure you have docker (see https://docs.docker.com/engine/installation) and docker-compose (see https://docs.docker.com/compose/install) installed


Getting started
---------------

1. clone this repository
2. `cd lvm-roca-prototype`
3. run `git submodule update --init`
4. run `docker-compose up` (and grab a cup of coffee)
5. visit http://localhost:3000


Applications
------------

LVM roca-prototype consist of 5 different apps (mounted as git submodule). Each app is running in its own docker container.

1. lvm-las-roca: Main app and entrypoint (node/express)
  * visit http://localhost:3000
2. lvm-las-postbox: postbox/tasklist application (java/spring-mvc)
  * visit http://localhost:3001
3. lvm-las-letter: business letter (wizard) app (node/express)
  * visit http://localhost:3002
4. lvm-las-damage: damage/claim application (node/express)
  * visit http://localhost:3003
5. prototype-backend: backend mock
  * visit http://localhost:8080
  * visit sample partner data http://localhost:8080/partner/4711
