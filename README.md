ECGALAXY containers_toolbox role
================================

Ansible role which installs tools required to work with containers, image registries and Kubernetes clusters.

List of tools:

- argocd
- cosign
- dive
- eksctl
- helm
- k9s
- kpack CLI (kp)
- kubectl
- kubeseal
- pack
- regctl
- skopeo (*)

(*) Skopeo installation not yet supported on Amazon Linux 2 and Ubuntu before 22.04 LTS.

Requirements
------------

- The `unzip` command, which can be provided by the `ecgalaxy.common_packages` role.

Role Variables
--------------

For the list of all the available variables check the files under `defaults/` and `vars/`.

Dependencies
------------

- optional: ecgalaxy.common_packages

Example Playbook
----------------

    - hosts: all
      roles:
        - ecgalaxy.bootstrap
        - ecgalaxy.common_packages
        - ecgalaxy.containers_toolbox

License
-------

Copyright the European Union 2022.

Licensed under the EUPL-1.2 or later.

Author Information
------------------

ECGALAXY team.
