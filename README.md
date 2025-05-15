### "reimagined-dollop"

It's a Github-generated repository name, but the purpose of this repo is to deploy a dockerized Valheim server on a local Debian-based linux system with Ansible (ansible-pull)

#### Development

All the relevant Ansible code is in `local.yml`. Varialbes are in `group_vars/all.yml` and the Docker compose specs are in `valheim.docker-compose.yml`

#### Deployment

Since we are using `ansible-pull`, the setup will be deployed to localhost

##### Complete

```sh
ansible-pull -U https://github.com/mruokola/reimagined-dollop.git
```

##### Setup

```sh
ansible-pull -U https://github.com/mruokola/reimagined-dollop.git -t setup
```

##### Valheim only

```sh
ansible-pull -U https://github.com/mruokola/reimagined-dollop.git -t valheim -e valheim_server_password='mypassword'
```
