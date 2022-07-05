# ansible
users:
  - root
  - user1 (unprivileged)
  - admin2 (privileged)

 Privilege escalation:
  - become

Privilege escalation methods:
  - sudo
  - su
  - others, e.g. dzdo (won't discuss them here)

Privilege escalation requires password

Scenarios:

  - Running playbook as root
    - check permissions in admin2
  - Running playbook as privileged user (admin2)
  - Running playbook as unprivileged user (user1)


Another option:
  - use the "remote_user" variable
Caution: it is overriden by the "ansible_user" variable

Mapping privilege escalation options to Ansible Tower GUI
  