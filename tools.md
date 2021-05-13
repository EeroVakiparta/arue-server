  # docker
  ```
   39  sudo yum install -y yum-utils
   40  sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
   41  sudo yum install docker-ce docker-ce-cli containerd.io
   42  sudo systemctl start docker
   43  docker ps
   49  sudo systemctl enable docker
  ```
# docker-compose
```
    3  sudo yum update
    4  sudo yum upgrade
    5  curl
    6  sudo curl -L "https://github.com/docker/compose/releases/download/1.24.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
    7  sudo chmod +x /usr/local/bin/docker-compose
    8  docker–compose –-version
```

# htop

- Fancier version of the top, showing core specific loads.
- https://linuxhint.com/centos_install_htop/

```
sudo yum install epel-release
sudo yum update
sudo yum install htop
```

# emacs

- console IDE

```
yum install emacs
```

# screen

- session tool

```
sudo yum install screen
```

# ansible

```
sudo yum install ansible
```
