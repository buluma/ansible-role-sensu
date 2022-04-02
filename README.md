# [sensu](#sensu)

Installs and configures latest sensu

|GitHub|GitLab|Quality|Downloads|Version|Issues|Pull Requests|
|------|------|-------|---------|-------|------|-------------|
|[![github](https://github.com/buluma/ansible-role-sensu/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-sensu/actions)|[![gitlab](https://gitlab.com/buluma/ansible-role-sensu/badges/master/pipeline.svg)](https://gitlab.com/buluma/ansible-role-sensu)|[![quality](https://img.shields.io/ansible/quality/58624)](https://galaxy.ansible.com/buluma/sensu)|[![downloads](https://img.shields.io/ansible/role/d/58624)](https://galaxy.ansible.com/buluma/sensu)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-sensu.svg)](https://github.com/buluma/ansible-role-sensu/releases/)|[![Issues](https://img.shields.io/github/issues/buluma/ansible-role-sensu.svg)](https://github.com/buluma/ansible-role-sensu/issues/)|[![PullRequests](https://img.shields.io/github/issues-pr-closed-raw/buluma/ansible-role-sensu.svg)](https://github.com/buluma/ansible-role-sensu/pulls/)|

## [Example Playbook](#example-playbook)

This example is taken from `molecule/default/converge.yml` and is tested on each push, pull request and release.
```yaml
---
- name: converge
  hosts: all
  become: yes
  gather_facts: yes

  roles:
    - role: buluma.sensu
```

The machine needs to be prepared. In CI this is done using `molecule/default/prepare.yml`:
```yaml
---
- name: prepare
  hosts: all
  become: yes
  gather_facts: no

  roles:
    - role: buluma.bootstrap
    - role: buluma.epel
```

## [Requirements](#requirements)

- pip packages listed in [requirements.txt](https://github.com/buluma/ansible-role-sensu/blob/main/requirements.txt).


## [Context](#context)

This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.co.ke/) for further information.

Here is an overview of related roles:

![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-sensu/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/buluma):

|container|tags|
|---------|----|
|el|all|
|ubuntu|all|

The minimum version of Ansible required is 2.1, tests have been done to:

- The previous version.
- The current version.
- The development version.



If you find issues, please register them in [GitHub](https://github.com/buluma/ansible-role-sensu/issues)

## [License](#license)

Apache-2.0

## [Author Information](#author-information)

[Michael Buluma](https://buluma.github.io/)
