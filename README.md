Ansible role: Packer
=========

![Build & Deploy](https://github.com/Provizanta/ansible-role-packer/workflows/molecule/badge.svg?branch=master)

Establish and configure Packer.

Requirements
------------

None

Role Variables
--------------

No variables are defined in [defaults/main.yml](./defaults/main.yml).

Additionally, it is possible to define an explicit version to be downloaded and installed:

    packer_architecture: 'amd64'    # enum, one of 386|amd64|arm|arm64|mips|mips64|mipsle|ppc64le|s390x

    packer_version: '1.5.5'

Dependencies
------------

None

Example Playbook
----------------

To get a default package:

    - name: Converge
      hosts: all
      roles:
        - role: packer


To get an explicit version:

    - name: Converge
      hosts: all
      roles:
        - role: packer
          vars:
            packer_version: '1.5.6'
            packer_architecture: amd64

License
-------

MIT

Author Information
------------------

Tibor Csóka
