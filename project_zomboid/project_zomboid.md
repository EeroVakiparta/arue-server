# Minecraft

## Reference

- https://github.com/itzg/docker-minecraft-server
- https://serialized.net/2021/02/minecraft_server_docker/


## START / RESTART

```
$cd /srv/minecraft/
docker-compose -f aruecraft.yml up -d
docker minecraft_mc_1 logs
```

```
$cd /srv/minecraft/
docker-compose -f aruecraft.yml up -d
```

### ports to be forwarder
25565 - 25565	TCP	
25575 - 25575	TCP	


## MAINTENACE

### Log files

Observerving logs
```
$cd ~/data/minecraft/logs/
$tailf latest.log
$less 2021-07-27-3.log.gz
$less * | grep WARN

```

### Server properties

Observerving logs
```
$cd ~/data/minecraft/

server.properties
```
requires restart

### World file 

```
$cd ~/data/minecraft/world/
```

### Ping tests:

```
PING
City center: 34 ms
Amsterdam: 45 ms
```

### TODO: study

https://cassiofernando.netlify.app/blog/minecraft-java-arguments
