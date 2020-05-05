[![Build Status](https://travis-ci.com/Mireiawen/ansible-role-hub.svg?branch=master)](https://travis-ci.com/Mireiawen/ansible-role-hub) [![Ansible Galaxy](https://img.shields.io/badge/Ansible%20Galaxy-mireiawen.hub-blueviolet)](https://galaxy.ansible.com/mireiawen/hub)


# Hub

Installs the GitHub command line package `hub`. Should work on most distributions.

## Requirements

None.

## Role Variables

### hub_package
The name of the Hub package to install. Defaults to `hub`

### hub_status
The status for the package. Defaults to `latest`

### hub_build_from_source
True if the package should be built from the source. Defaults to false in most cases, true for RedHat and Alpine.

### hub_source_version
The version to install when using source. Defaults to `HEAD`

## Dependencies

None.

## Example Playbook

    - hosts: "servers"
      roles:
         - "mireiawen.hub"

## License
MIT, see `LICENSE`

