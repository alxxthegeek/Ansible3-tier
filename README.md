# Ansible3-tier
Ansible provisioning a 3 tier web app on AWS.

Assumes Ansible is fully setup with dynamic inventory.
Assumes that the playbook is being run from linux (fedora/centos/redhat)

All instances will run Amazon Linux.

Setup to be run in ap-southeast-2c (Sydney), if you need to change region
change the region and availability zones in group_vars/all/vars
