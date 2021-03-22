## ubuntu-1804-mariadb-server

Ansible role to set up a MariaDB server on Ubuntu 18.04.

#### Variables

* `ubuntu_1804_mariadb_server_root_password`: [required]: Root password

* `ubuntu_1804_mariadb_server_certificates_present`: [default: `{}`]: SSL certificates to create
* `ubuntu_1804_mariadb_server_certificates_absent`: [default: `[]`]: SSL certificates to remove

* `ubuntu_1804_mariadb_server_configuration_files_present`: [default: `{}`]: Configuration files to create
* `ubuntu_1804_mariadb_server_configuration_files_absent`: [default: `[]`]: Configuration files to remove

#### Examples

##### Minimal (set root password only)

```yaml
---
- hosts: all
  roles:
    - ubuntu-1804-mariadb-server
  vars:
    ubuntu_1804_mariadb_server_root_password: 'this-is-a-test-password'
```
