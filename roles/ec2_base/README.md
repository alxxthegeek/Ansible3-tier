webserver
===============

This role contains configuration that should be applied to all  instances

Requirements
------------

This role is expecting to be run on a Red Hat based system.  E.g. CentOS or Amazon Linux 2

Role Variables
--------------

      instance_type: a1.large
      security_group: ansible-webserver # security group name
      image: ami-0e98ccceff552e8a8      # ami you want to use for the instance/s
      keypair: keykey                   # pem file
      ansible_ssh_private_key_file: "~/.ssh/keykey.pem"
      key : "~/.ssh/id_rsa.pub"
      region: us-east-1                 # Change the Region
      count: 1                          # number of instances


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