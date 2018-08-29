# Python 3 custom Docker images

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Docker Build status](https://img.shields.io/docker/build/codeyourinfra/python3.svg)](https://hub.docker.com/r/codeyourinfra/python3/builds) [![Docker Pulls](https://img.shields.io/docker/pulls/codeyourinfra/python3.svg)](https://hub.docker.com/r/codeyourinfra/python3)

Linux distributions base Docker images with just Python 3 installed:

Distribution | Tag
------------ | ---
[Ubuntu 16.04 LTS](https://github.com/codeyourinfra/python3/blob/master/xenial/Dockerfile) | xenial
[Ubuntu 18.04 LTS](https://github.com/codeyourinfra/python3/blob/master/bionic/Dockerfile) | bionic

Use the tag to pull the specific Docker image: `docker pull codeyourinfra/python3:tag`.

The default command `tail -f /dev/null` executed on container initialization keeps it up when in detached mode.

The *bionic* image, for example, can so be instantiated by simply executing: `docker run --name bionic -d codeyourinfra/python3:bionic`.

A good usage for the **Python 3 custom Docker images** is for testing [Ansible roles](https://docs.ansible.com/ansible/latest/user_guide/playbooks_reuse_roles.html). The build process of each [Codeyourinfra's Ansible role](https://galaxy.ansible.com/codeyourinfra), for example, uses the images for testing.