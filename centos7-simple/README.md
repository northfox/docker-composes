centos7-simple
===

- [ref](https://qiita.com/TakashiOshikawa/items/081d4780abdc21d63b1a)
- [ref](https://blue21neo.blogspot.com/2017/01/sshdocker-dokerfile.html)

`docker-compose up -d --build`

## key settings for ssh
- `ssh-keygen -t rsa -b 4096 -f ~/.ssh/myvps_centos7_simple_id_rsa`
- `vim ~/.ssh/config`
```
Host myvps.centos7-simple
    HostName 0.0.0.0
    User root
    Port [SSH_PORT]
    IdentityFile ~/.ssh/myvps_centos7_simple_id_rsa
```
