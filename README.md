# ansible-role-install-bat

A role to install bat on all Linux x86_64 systeme from prebuilt binary.

## Role Variables

| Name                    | Type   | Required | Default          | Comment                               |
| ----------------------- | ------ | -------- | ---------------- | ------------------------------------- |
| bat_version             | string | false    | `0.15.0`         | Bat version to install                |
| bat_binary_install_path | string | false    | `/usr/local/bin` | Where the bat binary will be deployed |

## Example Playbook

```
- name: test playbook
  hosts: "my_host"
  gather_facts: no
  remote_user: my_user
  become: false

  roles:
    - role: ansible-role-install-bat
```

## License

MIT
