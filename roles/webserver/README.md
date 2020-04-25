webserver
===============

This role contains webserver configuration that should be applied to all webserver instances

Requirements
------------

This role is expecting to be run on a Red Hat based system.  E.g. CentOS or Amazon Linux 2

Role Variables
--------------

      ansible_ssh_common_args: "-o StrictHostKeyChecking=no"      
      ansible_ssh_user: "ec2-user"
      domain_name: www.qantastechops.com
      domain: qantastechops
      http_conf: qantastechops.conf
      http_port: 80
      disable_default: true


Dependencies
------------

None

Example Playbook
----------------

Just apply the role, and supply the required vars:

  - name: Install ql_common_linux and webserver roles
    hosts: launched
    become: True
    gather_facts: True
    vars:
      ansible_ssh_common_args: "-o StrictHostKeyChecking=no"      
      ansible_ssh_user: "ec2-user"
      domain_name: www.qantastechops.com
      domain: qantastechops
      http_conf: qantastechops.conf
      http_port: 80
      disable_default: true
    roles:
      - {role: webserver}

License
-------

Commercial

Author Information
------------------
