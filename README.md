arineng.epel
=========

An Ansible Role to Deploy EPEL for RHEL and RHEL Derivatives

Requirements
------------

None

Role Variables
--------------

From defaults/main.yml:
```
---
epel_repo_url: https://dl.fedoraproject.org/pub/epel/{{ ansible_distribution_major_version }}/{{ ansible_architecture }}
epel_repo_gpg_key_url: https://dl.fedoraproject.org/pub/epel/RPM-GPG-KEY-EPEL-{{ ansible_distribution_major_version }}
epel_repofile_path: /etc/yum.repos.d/epel
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: arineng.epel }

License
-------

BSD

