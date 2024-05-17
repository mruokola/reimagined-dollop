#### Deployment

##### Complete

```sh
ansible-pull -U https://github.com/mruokola/reimagined-dollop.git
```

##### Setup

```sh
ansible-pull -U https://github.com/mruokola/reimagined-dollop.git -t setup
```

##### Valheim

```sh
ansible-pull -U https://github.com/mruokola/reimagined-dollop.git -t valheim -e valheim_server_password='mypassword'
```
