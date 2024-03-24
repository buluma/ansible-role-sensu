# Ansible role [sensu](https://galaxy.ansible.com/ui/standalone/roles/buluma/sensu/documentation)

Installs and configures latest sensu

|GitHub|Version|Issues|Pull Requests|Downloads|
|------|-------|------|-------------|---------|
|[![github](https://github.com/buluma/ansible-role-sensu/actions/workflows/molecule.yml/badge.svg)](https://github.com/buluma/ansible-role-sensu/actions/workflows/molecule.yml)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-sensu.svg)](https://github.com/buluma/ansible-role-sensu/releases/)|[![Issues](https://img.shields.io/github/issues/buluma/ansible-role-sensu.svg)](https://github.com/buluma/ansible-role-sensu/issues/)|[![PullRequests](https://img.shields.io/github/issues-pr-closed-raw/buluma/ansible-role-sensu.svg)](https://github.com/buluma/ansible-role-sensu/pulls/)|[![Ansible Role](https://img.shields.io/ansible/role/d/buluma/sensu)](https://galaxy.ansible.com/ui/standalone/roles/buluma/sensu/documentation)|

## [Example Playbook](#example-playbook)

This example is taken from [`molecule/default/converge.yml`](https://github.com/buluma/ansible-role-sensu/blob/master/molecule/default/converge.yml) and is tested on each push, pull request and release.

```yaml
---
- name: Converge
  hosts: all
  become: yes
  gather_facts: yes

  roles:
    - role: buluma.sensu
```

The machine needs to be prepared. In CI this is done using [`molecule/default/prepare.yml`](https://github.com/buluma/ansible-role-sensu/blob/master/molecule/default/prepare.yml):

```yaml
---
- name: Prepare
  hosts: all
  become: yes
  gather_facts: no

  roles:
    - role: buluma.bootstrap
    - role: buluma.epel
    - role: buluma.ca_certificates
    - role: buluma.nginx
```

Also see a [full explanation and example](https://buluma.github.io/how-to-use-these-roles.html) on how to use these roles.

## [Role Variables](#role-variables)

The default values for the variables are set in [`defaults/main.yml`](https://github.com/buluma/ansible-role-sensu/blob/master/defaults/main.yml):

```yaml
---
# defaults file for ansible-sensu-install
```

## [Requirements](#requirements)

- pip packages listed in [requirements.txt](https://github.com/buluma/ansible-role-sensu/blob/master/requirements.txt).

## [State of used roles](#state-of-used-roles)

The following roles are used to prepare a system. You can prepare your system in another way.

| Requirement | GitHub | Version |
|-------------|--------|--------|
|[buluma.bootstrap](https://galaxy.ansible.com/buluma/bootstrap)|[![Ansible Molecule](https://github.com/buluma/ansible-role-bootstrap/actions/workflows/molecule.yml/badge.svg)](https://github.com/buluma/ansible-role-bootstrap/actions/workflows/molecule.yml)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-bootstrap.svg)](https://github.com/shadowwalker/ansible-role-bootstrap)|
|[buluma.epel](https://galaxy.ansible.com/buluma/epel)|[![Ansible Molecule](https://github.com/buluma/ansible-role-epel/actions/workflows/molecule.yml/badge.svg)](https://github.com/buluma/ansible-role-epel/actions/workflows/molecule.yml)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-epel.svg)](https://github.com/shadowwalker/ansible-role-epel)|
|[buluma.ca_certificates](https://galaxy.ansible.com/buluma/ca_certificates)|[![Ansible Molecule](https://github.com/buluma/ansible-role-ca_certificates/actions/workflows/molecule.yml/badge.svg)](https://github.com/buluma/ansible-role-ca_certificates/actions/workflows/molecule.yml)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-ca_certificates.svg)](https://github.com/shadowwalker/ansible-role-ca_certificates)|
|[buluma.nginx](https://galaxy.ansible.com/buluma/nginx)|[![Ansible Molecule](https://github.com/buluma/ansible-role-nginx/actions/workflows/molecule.yml/badge.svg)](https://github.com/buluma/ansible-role-nginx/actions/workflows/molecule.yml)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-nginx.svg)](https://github.com/shadowwalker/ansible-role-nginx)|

## [Context](#context)

This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.github.io/) for further information.

Here is an overview of related roles:

![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-sensu/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/buluma):

|container|tags|
|---------|----|
|[Ubuntu](https://hub.docker.com/r/buluma/ubuntu)|focal, bionic, jammy|

The minimum version of Ansible required is 2.1, tests have been done to:

- The previous version.
- The current version.
- The development version.

If you find issues, please register them in [GitHub](https://github.com/buluma/ansible-role-sensu/issues)

## [Changelog](#changelog)

[Role History](https://github.com/buluma/ansible-role-sensu/blob/master/CHANGELOG.md)

## [License](#license)

[Apache-2.0](https://github.com/buluma/ansible-role-sensu/blob/master/LICENSE)

## [Author Information](#author-information)

[Shadow Walker](https://buluma.github.io/)

