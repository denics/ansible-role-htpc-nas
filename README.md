htpc-nas
===========
[![Build Status](https://travis-ci.org/denics/ansible-role-htpc-nas.svg?branch=master)](https://travis-ci.org/denics/ansible-role-htpc-nas)

An Ansible role to setup and configure NAS functionality ( NFS, CIFS and AFP ) for HTPC Server under Ubuntu.

Requirements
------------

This role requires Ansible 2.0 or higher. Platform requirements are listed in the metadata file.
Make sure to download roles specified in **Dependencies** section if role installed **not** with Ansible Galaxy.

Overview
--------

List of tasks that will be performed under `htpc-nas` role:

1. Configure NFS Server. Squash all users to `htpc_user_username` uid
2. Configure SAMBA Server. Create `htpc_user_username` samba identified by `htpc_user_password`
3. Configure AFP ( Netatalk ) server for sharing data with Macs.
