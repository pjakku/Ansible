Example variable:
time_zone: Eastern Standard Time (required time zone name)

model Play:
---
- host: all
  gather_facts: false
  roles:
  - role: Windows-timezone
    time_zone: Eastern Standard Time

Author Information
------------------
Praveen Jakku
