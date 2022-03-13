# [cargo](#cargo)

Install cargo on your system.

|GitHub|GitLab|Quality|Downloads|Version|
|------|------|-------|---------|-------|
|[![github](https://github.com/buluma/ansible-role-cargo/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-cargo/actions)|[![gitlab](https://gitlab.com/buluma/ansible-role-cargo/badges/master/pipeline.svg)](https://gitlab.com/buluma/ansible-role-cargo)|[![quality](https://img.shields.io/ansible/quality/)](https://galaxy.ansible.com/buluma/cargo)|[![downloads](https://img.shields.io/ansible/role/d/)](https://galaxy.ansible.com/buluma/cargo)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-cargo.svg)](https://github.com/buluma/ansible-role-cargo/releases/)|

## [Example Playbook](#example-playbook)

This example is taken from `molecule/default/converge.yml` and is tested on each push, pull request and release.
```yaml
---
- name: Converge
  hosts: all
  become: yes
  gather_facts: yes

  roles:
    - role: buluma.cargo
```

The machine needs to be prepared. In CI this is done using `molecule/default/prepare.yml`:
```yaml
---
- name: Prepare
  hosts: all
  become: yes
  gather_facts: no

  roles:
    - role: buluma.bootstrap
    - role: buluma.buildtools
```


## [Role Variables](#role-variables)

The default values for the variables are set in `defaults/main.yml`:
```yaml
---
# defaults file for cargo

# The destination where cargo should be installed.
cargo_prefix: /usr/local

# Where to drop the downloaded installer.
cargo_tmp: /root
```

## [Requirements](#requirements)

- pip packages listed in [requirements.txt](https://github.com/buluma/ansible-role-cargo/blob/main/requirements.txt).

## [Status of used roles](#status-of-requirements)

The following roles are used to prepare a system. You can prepare your system in another way.

| Requirement | GitHub | GitLab |
|-------------|--------|--------|
|[robertdebock.bootstrap](https://galaxy.ansible.com/buluma/robertdebock.bootstrap)|[![Build Status GitHub](https://github.com/buluma/robertdebock.bootstrap/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/robertdebock.bootstrap/actions)|[![Build Status GitLab ](https://gitlab.com/buluma/robertdebock.bootstrap/badges/master/pipeline.svg)](https://gitlab.com/buluma/robertdebock.bootstrap)|
|[robertdebock.buildtools](https://galaxy.ansible.com/buluma/robertdebock.buildtools)|[![Build Status GitHub](https://github.com/buluma/robertdebock.buildtools/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/robertdebock.buildtools/actions)|[![Build Status GitLab ](https://gitlab.com/buluma/robertdebock.buildtools/badges/master/pipeline.svg)](https://gitlab.com/buluma/robertdebock.buildtools)|
|[robertdebock.epel](https://galaxy.ansible.com/buluma/robertdebock.epel)|[![Build Status GitHub](https://github.com/buluma/robertdebock.epel/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/robertdebock.epel/actions)|[![Build Status GitLab ](https://gitlab.com/buluma/robertdebock.epel/badges/master/pipeline.svg)](https://gitlab.com/buluma/robertdebock.epel)|

## [Context](#context)

This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.co.ke/) for further information.

Here is an overview of related roles:

![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-cargo/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/buluma):

|container|tags|
|---------|----|
|alpine|all|
|amazon|Candidate|
|el|8|
|debian|all|
|fedora|all|
|opensuse|all|
|ubuntu|all|

The minimum version of Ansible required is 2.10, tests have been done to:

- The previous version.
- The current version.
- The development version.



If you find issues, please register them in [GitHub](https://github.com/buluma/ansible-role-cargo/issues)

## [License](#license)

Apache-2.0

## [Author Information](#author-information)

[Michael Buluma](https://buluma.github.io/)
