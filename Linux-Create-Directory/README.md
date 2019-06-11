
Variable:::
------------
directory_structure: Target directory path for this change
dir_permission: Target directory permission mode (ex.0755)
dir_recursive: Recursively set directory permission attributes
dir_user_name: Username for the directory ownership (local/kerbirized user)
dir_group_name: Groupname for the directory ownership (local/kerborized group)

Model Play to add in PB
-----------------------

---
- name: 'create Directory'
  hosts: all
roles:
  - role: Linux-Create-Directory
    targetdir_lists:
       - { directory_structure: '/tmp/test/', dir_permission: '0755' , dir_recursive: 'yes' , dir_user_name: 'root' , dir_group_name: 'root' }
       - { directory_structure: '/tmp/dest/', dir_permission: '0755' , dir_recursive: 'no' , dir_user_name: '' , dir_group_name: '' }
....

Author Information
------------------
Praveen Jakku
