Install AWX on CentOS without Docker with this simple Ansible role.

Prerequisite : 
-ansible 
-epel-release 
-internet connection

Each task is labbeled and you'll also find repos and nginx configuration in the template folders.

You'll need to place the folder "AWX_Install" in /etc/ansible/roles/ for this to work. If your ansible folder is located somewhere else just mkdir /etc/ansible/roles.

/!\ SECURITY WARNING: Do not forget to edit "7-awx.yml" (line 19) or "main.yml" (l 171) to include your username and password  otherwise you'll have default "admin" user and "password". /!\

This might be added as a var in the future.


Instructions to install AWX without docker can be found here : https://raw.githubusercontent.com/faudeltn/AnsibleTower-awx/master/ansible-awx-install/install-awx

My contribution is just a simple Ansible script to install AWX and it's dependencies so you don't have to.

Special thanks to Mrmeee and Warden Lofti for their contributions to AWX.
