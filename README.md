Ansible role: Packer
=========

[![Build Status](https://travis-ci.com/Provizanta/ansible-role-packer.svg?branch=master)](https://travis-ci.com/Provizanta/ansible-role-packer)

Establish and configure Packer.

Requirements
------------

None

Role Variables
--------------

These variables are defined in [defaults/main.yml](./defaults/main.yml):

    packer_architecture: 'amd64'    # enum, one of 386|amd64|arm|arm64|mips|mips64|mipsle|ppc64le|s390x

    packer_version: '1.5.5'

    packer_binary_dir_path: "/usr/local/bin"


Dependencies
------------

None

Example Playbook
----------------

    - name: Converge
      hosts: all
      roles:
        - role: packer
          vars:
            packer_binary_dir_path: /usr/bin

License
-------

MIT

Author Information
------------------

Tibor Csóka
