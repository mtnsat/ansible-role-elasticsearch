# Ansible Role: Elasticsearch

[![Build Status](https://travis-ci.org/mtnsat/ansible-role-elasticsearch.svg?branch=master)](https://travis-ci.org/mtnsat/ansible-role-elasticsearch)

An Ansible Role that installs Elasticsearch on RedHat/CentOS or Debian/Ubuntu.

## Requirements

None.

## Role Variables

- aws_install: true : installs and configures cloud-aws plugin

## Dependencies

  - mtn_oracle_java

## Example Playbook

    - hosts: search
      roles:
        - role: mtnsat.elasticsearch
          elasticsearch_version: 2.3.2

All nodes in an elasticsearch cluster must have matching versions. Replication fails to nodes with lower minor versions.

## License

MIT / BSD

## Author Information

This role was created in 2014 by [Jeff Geerling](http://jeffgeerling.com/), author of [Ansible for DevOps](http://ansiblefordevops.com/).
