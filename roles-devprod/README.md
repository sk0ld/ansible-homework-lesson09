It's a very simple example of ansible roles usage
=========

Short info
------------

Tested on Ubuntu 20.04

dev host is for preparation of war file with maven

prod host is for publishing war file by tomcat

Requirements
------------

Tested with root credentials.
ssh key exchange is needed:
1) Between ansible master and both nodes.
2) Between dev node and prod node.
3) Between prod node and dev node.

Usage
--------------

ansible-playbook /path-to/roles-devprod/roles-devprod.yml


Example of /etc/ansible/hosts
-----------------------------

```
[dev]
devserver1 ansible_host=your_ip_or_fqdn_devserver1

[prod]
prodserver1 ansible_host=your_ip_or_fqdn_prodserver1

```