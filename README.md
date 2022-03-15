# Chain-Infra
our chain infrastructure

## Installation
```shell
$ brew install ansible
```

## Prepare
Copy `ansible/defaults/main.yml.example` to `ansible/defaults/main.yml` and define configs about aws setting.
```shell
$ cp ansible/defaults/main.yml.example ansible/defaults/main.yml
```

## Use it
```shell
$ cd ansible && ansible-playbook create_ourchain.yml
```