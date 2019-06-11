Package_name: name of the packageor file to be downloaded and unarchive
target_dir: path of the directory where the package to be extracted.

Model PB::
----------

---
- host: all
  gather_facts: false
  roles:
    - role: linux-extract-artifacory
      target_dir: '/usr/abc'
      package_name: 'jdk.tar.gz'


Author Information
------------------
Praveen Jakku
