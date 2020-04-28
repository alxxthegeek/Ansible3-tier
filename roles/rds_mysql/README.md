ec2_key
===============

This role generates a new ec2 keypair and saves it to the users .ssh directory

Requirements
------------



Role Variables
--------------

      keypair
      region


Dependencies
------------

None

Example Playbook
----------------

Just apply the role, and supply the required vars:

  - name: test
    vars:
      region: ap-southeast-2     
      keypair: awskeyname
    roles:
      - {role: ec2_key}

License
-------

BSD

Author Information
------------------

Alex Gibson