# arue-server

- Just gathering notes...

https://www.bogotobogo.com/DevOps/Docker/Docker_Prometheus_Grafana.php
https://github.com/stefanprodan/dockprom

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
