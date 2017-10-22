## ubuntu-1604-mariadb-server

Set up a MariaDB server on Ubuntu 16.04.

#### Variables

* `ubuntu_1604_mariadb_server_root_password`: [required]: Root password

* `ubuntu_1604_mariadb_server_certificates_present`: [default: `{}`]: SSL certificates to create
* `ubuntu_1604_mariadb_server_certificates_absent`: [default: `[]`]: SSL certificates to remove

* `ubuntu_1604_mariadb_server_configuration_files_present`: [default: `{}`]: Configuration files to create
* `ubuntu_1604_mariadb_server_configuration_files_absent`: [default: `[]`]: Configuration files to remove

#### Examples

##### Minimal (set root password only)

```yaml
---
- hosts: all
  roles:
    - percona-server
  vars:
    ubuntu_1604_mariadb_server_root_password: 'this-is-a-test-password'
```
