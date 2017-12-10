Role Name: Utils
================

I am using this role when I need to setup a new server.

Requirements
------------

No requirements

Role Variables
--------------

The list of packages to install must be listed in the playbook  

Dependencies
------------

No dependencies

Installation
------------

You can get this role by using ```git clone``` command.  
You can also add this repo to your ```requirements.yml``` and use ```ansible-galaxy install -r requirements.yml -p {{path_to_roles}}```  
Or you can download the zip and unzip it in your roles directory 

Example Playbook
----------------

Here is an example of my test playbook.

```---
   - name: Demo
     hosts:
       - web-debian
       - web-centos
     roles:
       - utils
     vars:
       apps:
         - python-pip
         - git
         - tig
         - curl
         - htop
         - zsh
         - vim
         - telnet
         - wget
         - unzip
 ```

License
-------

BSD

