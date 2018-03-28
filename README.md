# ansible-role-protobuf

Ansible role for Google protocol buffers.

## Status

[![galaxy](https://img.shields.io/ansible/role/24647.svg?style=for-the-badge)](https://galaxy.ansible.com/ricardogama/protobuf/) [![license](https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge)](https://raw.githubusercontent.com/ricardogama/ansible-role-protobuf/master/LICENSE)

## Installation

Install this role via Galaxy:

```sh
$ ansible-galaxy install ricardogama.protobuf
```

## Variables

Override the protobuf distribution if necessary:

```yaml
protobuf_src: https://github.com/google/protobuf/releases/download/v3.5.1/protoc-3.5.1-linux-x86_64.tar.gz
```

Below is the default directory where the protobuf distribution will be saved to:

```yaml
protobuf_dest: /usr/local/protoc
```

## Playbook example

Just add `ricardogama.protobuf` to your playbook roles:

```yaml
- hosts: localhost
  roles:
    - ricardogama.protobuf
```
