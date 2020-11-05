# Ansible Role: group

An Ansible Role to create/update groups.

[![Actions Status](https://github.com/tristan-weil/ansible-role-group/workflows/molecule/badge.svg?branch=master)](https://github.com/tristan-weil/ansible-role-group/actions)

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

Mandatory variables:

| Variable      | Description |
| :------------ | :---------- |

Optional variables:

| Variable      | Default | Description |
| :------------ | :------ | :---------- |
| group_list    | []      | a list of <*group entry*> |

### <*group entry*>

Mandatory variables:

| Variable      | Description |
| :------------ | :---------- |
| name          | the group name |

Optional variables:

| Variable      | Default | Description |
| :------------ | :------ | :---------- |
| system        | False   | *True / False*: to create a system group |

## Example Playbook

    - hosts: 'webservers'
      roles:
        - role: 'ansible-role-group'
          group_list:
            - name: 'group1'

## Todo

None.

## Dependencies

None.

## Supported platforms

See [meta/main.yml](https://github.com/tristan-weil/ansible-role-group/blob/master/meta/main.yml)

## License

See [LICENSE.md](LICENSE.md)
