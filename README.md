![Build Status](https://img.shields.io/gitlab/pipeline-status/mireiawenrose/ansible-roles/hub?branch=master&style=plastic) [![Ansible Galaxy](https://img.shields.io/badge/Ansible%20Galaxy-mireiawen.hub-blueviolet?style=plastic)](https://galaxy.ansible.com/mireiawen/hub)


# Hub
Installs the GitHub command line package `hub`. Should work on most distributions.

## Requirements
None.

## Role Variables
 Configuration key       | Description                              | Default value
-------------------------|------------------------------------------|----------------------
 `hub_package`           | The name of the package to install       |`hub`
 `hub_status`            | The desired status for the package       | `latest`
 `hub_build_from_source` | Should the package be built from sources | false in most cases, true for RedHat and Alpine.
 `hub_source_version`    | The source version to install            | `HEAD`

## Dependencies
* community.general

## Example Playbook
```yaml
- hosts: "servers"
  roles:
  - "mireiawen.hub"
```

## License
MIT, see `LICENSE`
