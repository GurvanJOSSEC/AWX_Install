AWX_Install (Dockerless, automated installation of AWX)
=========

This role helps you Install a dockerless AWX server using ansible. 
The role is meant to be applied directly on the ansible server 



This role will install :

-policycoreutils-python

-rabbitmq-server

-rh-git29

-postgresql10 (server/contrib/libs)

-rh-postgresql10

-memcached

-nginx

-rh-python36

-ansible-awx



You'll need to place the folder "AWX_Install" in /etc/ansible/roles/ for this to work. If your ansible folder is located somewhere else just mkdir /etc/ansible/roles.


Then run the command : 

ansible-playbook /etc/ansible/roles/AWX_Install/tasks/main.yml

You can also run parts specific tasks : 

ansible-playbook /etc/ansible/roles/AWX_Install/tasks/1-AWX_repo_dependancies.yml




/!\ SECURITY WARNING /!\ :

You need to change the password and username in main.yml (line 171) or in 7-Awx.yml (l 19) 
Otherwise the default (admin/password) will be used. 

Requirements
------------

-Ansible
-Epel-Release
-Internet Connection

Role Variables
--------------

Nothing for now

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.


License
-------

opensource

Author Information
------------------
Gurvan JOSSEC
Infrastructure Engineer 

https://github.com/GurvanJOSSEC/
https://www.linkedin.com/in/gurvan-jossec/

Special thanks to MrMeee and Waderni Lotfi for their contribution to AWX. 

Instructions to install AWX (dockerless) : https://raw.githubusercontent.com/faudeltn/AnsibleTower-awx/master/ansible-awx-install/install-awx
