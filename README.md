RHEL 7 DISA STIG
================




Requirements
------------

RHEL 7. Other versions are not supported.

Role Variables
--------------

| Name              | Default Value       | Description          |
|-------------------|---------------------|----------------------|
| `rhel7stig_cat1_audit` | 'yes' | Audit for CAT I findings      |
| `rhel7stig_cat2_audit` | 'no'  | Audit for CAT II findings     |
| `rhel7stig_cat3_audit` | 'no'  | Audit for CAT III findings    |
| `rhel7stig_cat1_patch` | 'yes' | Correct CAT I findings        |
| `rhel7stig_cat2_patch` | 'no'  | Correct CAT II findings       |
| `rhel7stig_cat3_patch` | 'no'  | Correct CAT III findings      |


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
