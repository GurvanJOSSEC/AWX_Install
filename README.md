# AWX_Install
Install AWX on CentOS without Docker with this simple Ansible role. 

Each task is labbeled and you'll also find repo and nginx configuration in the template folders. 

You'll need to place the folder "AWX_Install" in /etc/ansible/roles/ for this to work.

/!\ At this moment everything works except for "rh-python36*" installation. /!\

So you'll need to do it manually. (see point number 5 on Wardeni's article) 

This will be fixed in the future. 


/!\ Do not forget to edit "7-awx.yml" to include your username and password (line 19) otherwise you'll have default "admin" user and "password". /!\


Instructions to install AWX without docker can be found here :
https://raw.githubusercontent.com/faudeltn/AnsibleTower-awx/master/ansible-awx-install/install-awx

My contribution is just a simple Ansible script to install AWX and it's dependencies so you don't have to. 

Special thanks to Mrmeee and Warden Lofti for their contributions.
