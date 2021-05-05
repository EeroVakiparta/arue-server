# Mumble

- https://github.com/PHLAK/docker-mumble

### setting SuperUser pw
```
docker exec -it mumble-server supw
```

### to configure server:
https://wiki.mumble.info/wiki/Murmur.ini
```
docker exec -it mumble-server vi /etc/mumble/config.ini
```

### useful commands
```
docker restart mumble-server
```