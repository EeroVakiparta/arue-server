# arue-server

# docker-compose
```
    3  sudo yum update
    4  sudo yum upgrade
    5  curl
    6  sudo curl -L "https://github.com/docker/compose/releases/download/1.24.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
    7  sudo chmod +x /usr/local/bin/docker-compose
    8  docker–compose –-version
```

# valheim
```
   11  mkdir -p $HOME/valheim-server/config $HOME/valheim-server/data
   12  cd $HOME/valheim-server/
   13  cat > $HOME/valheim-server/valheim.env << EOF
   14  SERVER_NAME=Arueheim
   15  WORLD_NAME=Arueheim
   16  SERVER_PASS=arue*****
   17  SERVER_PUBLIC=true
   18  EOF
   19  curl -o $HOME/valheim-server/docker-compose.yaml https://raw.githubusercontent.com/lloesche/valheim-server-docker/main/docker-compose.yaml
   20  docker-compose up
   
   22  sudo yum install -y yum-utils
   23  sudo yum update

   33  vi /etc/sysconfig/network-scripts/ifcfg-enp0s26f1u2
   34  service network restart
   35  nmcli d
   36  dhclient

   38  yum update
```  
  # docker
  ```
   39  sudo yum install -y yum-utils
   40  sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
   41  sudo yum install docker-ce docker-ce-cli containerd.io
   42  sudo systemctl start docker
   43  docker ps
   49  sudo systemctl enable docker
  ```

# OPENSSH ssh port and valheim ports
```
   45  sudo yum –y install openssh-server openssh-clients
   46  sudo systemctl start sshd
   47  sudo systemctl status sshd
   48  sudo systemctl enable sshd

   50  yum install vim
   51  sudo vim /etc/sysconfig/iptables
   52  sudo vim /etc/ssh/sshd_config

   54  vi /etc/sysconfig/network-scripts/ifcfg-enp0s26f1u2
   55  firewall-cmd --zone=public --add-port=22/tcp --permanent
   56  firewall-cmd --reload
   57  iptables-save | grep 22
   58  firewall-cmd --zone=public --add-port=2456-2458/udp --permanent
   59  firewall-cmd --reload
   60  systemctl start firewalld
   61  iptables-save
   62  ip addr
   63  sudo vim /etc/ssh/sshd_config
   64  service sshd restart
   65  service sshd start
   66  service sshd status
   67  firewall-cmd --zone=public --add-port=2222/tcp --permanent
   68  firewall-cmd --reload
   69  sudo vim /etc/ssh/sshd_config
   70  semanage port -a -t ssh_port_t -p tcp 2222
   71  service sshd restart
   72  service sshd status
   73  ip addr
```
# Restart
```
  113  shutdown --reboot
```
