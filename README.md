# Ansible

Introduction:
Ansible is an open-source software provisioning, configuration management, and application-deployment tool enabling infrastructure as code. 
It runs on many Unix-like systems, and can configure both Unix-like systems as well as Microsoft Windows. It aims to provide large productivity gains to a wide varietry of automation challesges.

Ansible Tower Framework by Redhat.
Ansible Tower (formerly 'AWX') is a web-based solution that makes Ansible even more easy to use for IT teams of all kinds. It's designed to be the hub for all of your automation tasks. ... Tower is free for usage for up to 10 nodes, and comes bundled with amazing support from Ansible, Inc.


Ansible is agentless tool.
Communicates through SSH.
It uses playbook as the code storage bucket.


Ansible uses push mechanism to do the operations.





DEMO:
Set Up Lab Environment for Ansible:

Ansible in AWS Console:

sudo amazon-linux-extras install ansible2

yum install git python python-level python-pip openssl -y

open the vi editor to open hosts file:

vi /etc/ansible/hosts

create a group with private IP address of the hosts under ungrouped:

[demo]
IPv4(private Ips of the nodes)


Open aisuble configuration file:

vi /etc/ansible/ansible.cfg

change the file execution mode if the file is not executable:

chmod +x /etc/ansible/ansible.cfg


2-user]# adduser ansible
[root@ip-172-31-35-13 ec2-user]# passwd ansible 
Changing password for user ansible.
New password: 
Retype new password: 
passwd: all authentication tokens updated successfully.
[root@ip-172-31-35-13 ec2-user]# 


To give previlege to user got to visudo file and add user in root premission: ansible ALL=(ALL) NOPASSWD: ALL


To establish a connection with node got to ssh configuration file: vi /etc/ssh/sshd_config



