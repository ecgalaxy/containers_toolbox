ECGALAXY containers_toolbox role
========

Ansible role which installs tools required to work with containers.

List of tools:

- cosign
- dive
- eksctl
- helm
- k9s
- kapp
- kubectl
- kubeseal
- pack
- ytt

Requirements
------------

None.

Role Variables
--------------

For the list of all the available variables check the files under `defaults/` and `vars/`.

Dependencies
------------

- ecgalaxy.common_packages

Example Playbook
----------------

    - hosts: all
      roles:
        - ecgalaxy.common_packages
        - ecgalaxy.containers_toolbox

License
-------

Copyright the European Union 2022.

Licensed under the EUPL-1.2 or later.

Author Information
------------------

ECGALAXY team.
