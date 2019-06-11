Variable:
----------
rpms_list:: list the required packages to be installed.

Model Play:
----------
---
- host: all
  gather_facts: true
  
  roles:
- name: install rpms
  role: Linux-Yum
  rpms_list:
    - ansible  


Author Information
------------------
Praveen Jakku
