Windows-command
---------------
Variables:
command: windows command to run
path: destination path to run the command

Example PlayBook: 
-----------------
- name: 'windows command module'
  hosts: all
  roles:
     - role: "{{ playbook_dir }}"
       command_list:
  	  - { command: 'whoami', path: 'c:\' }
	  - { command: 'whoami' }

Author:
Praveen Jakku
