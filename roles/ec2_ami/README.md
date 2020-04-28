ec2_ami
===============

This role creates an ami from the supplied instances

Requirements
------------

This role is expecting to be run on a Red Hat based system.  E.g. CentOS or Amazon Linux 2

Role Variables
--------------

      region: us-east-1
      ami_name: ql-ansible-arm64-a1-large-abcd1234

Dependencies
------------

None

Example Playbook
----------------

Just apply the role, and supply the required vars:

    roles:
    - {role: ec2_base}

License
-------

Commercial

Author Information
------------------

Alex Gibson