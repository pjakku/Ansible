To Execute the the shell commands or scripts on any Windows servers.

command_name	          generic			powershell command or path to powershell scripts
path			  C:\somedir		        set the spesfific path before executing a command
executable		  cmd			        change the shell used to execute the command (eg, cmd).

****Sample PlayBook****
-----------------------
---
- hosts: all
  gather_facts: false
  roles:
  - role: "{{ playbook_dir }}"
  list:
  - { command_name: 'value' }
  - { command_name: 'value2', path: 'script/path', executable: 'cmd' }


