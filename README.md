RHEL 7 DISA STIG
================

Based on [Red Hat Enterprise Linux 7 STIG Version 1 Release 0.2 - 2015-01-23](http://iasecontent.disa.mil/stigs/zip/U_Red_Hat_Enterprise_Linux_7_V1R0-2_IDraftSTIG.zip)

The best method for viewing the STIGS are via [Stig Viewer](http://iase.disa.mil/stigs/Pages/stig-viewing-guidance.aspx)

This repo originated from work done by [Sam Doran & Josh Springer](https://github.com/samdoran/ansible-role-rhel7stig)

Requirements
------------

RHEL 7. Other versions are not supported.
Ansible Version 2.1+. Previous versions are not supported.

Role Variables
--------------

| Name              | Default Value       | Description          |
|-------------------|---------------------|----------------------|
| `rhel7stig_cat1_patch` | True | Correct CAT I findings |
| `rhel7stig_cat2_patch` | False | Correct CAT II findings |
| `rhel7stig_cat3_patch` | False | Correct CAT III findings |

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: rhel7-stig, when: "ansible_os_family == 'RedHat' and ansible_os_major_verision == 7"}

License
-------

MIT
