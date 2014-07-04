Vagrant Docker
==============

A vagrant provision of a base ubuntu 14.04 (3.13 kernel) with docker already installed

This is just a wrapper for the vagrant docker image at: 
https://oss-binaries.phusionpassenger.com/vagrant/boxes/

Installs:
* lxc-docker (as this is docker-io)
* git (so you can clone docker images)

Usage
------

* Git clone the repository
* run ```vagrant up```
    * This will create a new VM on IP ```2.2.2.2```
* To ssh into the VM use ```vagrant ssh```
    * (if required) password: ```vagrant```
* Test docker with: ```sudo docker run ubuntu /bin/echo hello world```
