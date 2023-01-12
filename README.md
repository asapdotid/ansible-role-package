<p align="center"> <img src="https://user-images.githubusercontent.com/34257858/129839002-15e3f2c7-3f75-46d4-afae-0fd207d7fdde.png" width="100" height="100"></p>

<h1 align="center">
    Ansible Role Package
</h1>

<p align="center" style="font-size: 1.2rem;">
    This ansible role setup install packages On Ubuntu, CentOS, Redhat, Gento, Fedore, MacOS, ArchLinux, OpenSUSE
</p>

<p align="center">

<a href="https://www.ansible.com">
  <img src="https://img.shields.io/badge/Ansible-2.10-green?style=flat&logo=ansible" alt="Ansible">
</a>
<a href="LICENSE.md">
  <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="Licence">
</a>

## Requirements

None

## Role Variables

| Name               | Default Value | Description                                 |
| ------------------ | ------------- | ------------------------------------------- |
| `apt_repositories` | `[]`          | Debian repository.                          |
| `package_list`     | `[]`          | Package application install or remove list. |

## Dependencies

None.

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
- hosts: servers
  vars:
    package_list:
      - name: wget
      - name: htop
        state: present

  roles:
    - { role: asapdotid.package }
```

## License

MIT / BSD

## Author Information

[JogjaScript](https://jogjascript.com)

This role was created in 2021 by [Asapdotid](https://github.com/asapdotid).
