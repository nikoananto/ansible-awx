# Ansible Tower

## What is Ansible Tower ?

Ansible Tower is the enterprise version of Ansible, and it helps organizations and teams scale quickly and effectively. There is a cost associated with adopting it, installing it, and getting the software up and running in your environments. Ansible Tower offers more control than the free version and is a great platform for breaking down silos, as it can be used cross-functionally in an efficient manner.
Ansible Tower may be the more familiar option for Ansible users as it is the commercial GUI Ansible tool that provides the officially supported GUI interface, API access, role-based access, scheduling, notifications, and other nice features that allow businesses to manage environments easily with Ansible.

Ansible Tower requires a license to use the software. There is a trial license available for free that allows you and your teams to take Tower for a spin.
Tower currently only runs on the following distributions:
 - Red Hat Enterprise Linux (RHEL) 7 and 8
 - CentOS 6 and 7
 - Ubuntu 16.04

## What is Ansible AWX ?
Ansible AWX is the open-sourced project that was the foundation on which Ansible Tower was created. With this being said, Ansible AWX is a development branch of code that only undergoes minimal testing and quality engineering testing.
AWX provides a web-based user interface, REST API, and task engine built on top of Ansible. It is one of the upstream projects for Red Hat Ansible Automation Platform.

Perhaps the greatest benefit of AWX over Tower is that you have all of the enterprise features for an unlimited number of nodes. You are not limited by the free ’10-node’ limit for Ansible Tower. Basically, one of the major differences you will see between AWX and Tower is a different logo for the products. They look extremely similar.

Ansible AWX prerequisites
- Ansible Requires Version 2.8+
- Docker
  - A recent version
- docker Python module
  - This is incompatible with docker-py. If you have previously installed docker-py, please uninstall it.
  - We use this module instead of docker-py because it is what the docker-compose Python module requires.
- community.general.docker_image collection
  - This is only required if you are using Ansible >= 2.10
- GNU Make
- Git Requires Version 1.8.4+
- Python 3.6+
- Node 14.x LTS version
  - This is only required if you're building your own container images with use_container_for_build=false
- NPM 6.x LTS
  - This is only required if you're building your own container images with use_container_for_build=false
