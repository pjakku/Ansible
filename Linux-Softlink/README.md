
Variables:-
----------
source_name:   The source absolute path for which soft link needs to be created.
target_name:   The target absolute path of the soft link.
file_permission:  (Optional) Mode the file or directory should be
user_id:   (Optional) Name of the user that should own the file/directory, as would be fed to chown.
group_id: (Optional) Name of the group that should own the file/directory, as would be fed to chown.


Model PB::
-----------

---
- hosts: all
  gather_facts: false
  roles:
  - role: "{{ playbook_dir }}"
    source_name: "/app"
    target_name: "/usr/test"
    file_permission: 0755
    user_id: "userid"
    group_id: "groupid"


model play to main.yml with out user and group ID's:
----------------------------------------------------
---
- hosts: all
  gather_facts: false
  roles:
  - role: Linux-Softlink
    source_name: "/app"
    target_name: "/usr/test"
    


Author Information
------------------
Praveen Jakku
