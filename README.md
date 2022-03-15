# Chain-Infra
our chain infrastructure

## Prepare
Install ansible.
```shell
$ brew install ansible
```
Copy `ansible/defaults/main.yml.example` to `ansible/defaults/main.yml` and define configs about aws setting.
```shell
$ cp ansible/defaults/main.yml.example ansible/defaults/main.yml
```

## Use it
```shell
$ cd ansible && ansible-playbook create_ourchain.yml
```

## Record inventory
Write host into `ansible/inventory/hosts`. For example:
```
[ourchain]
ourchain-1 ansible_host=<ssh_connect_ip>
ourchain-2 ansible_host=<ssh_connect_ip>
```
