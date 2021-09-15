# Project Zomboid

## Reference

https://hub.docker.com/r/cyrale/project-zomboid
https://github.com/cyrale/project-zomboid


## START / RESTART

```
x
```

```
x
```

### ports to be forwarder
8766 - 8767 udp
16261 - 16272 udp

## MAINTENACE

### Server options

```
$vim /srv/projectzomboid/server-data/Server/aruezombi.ini
```

### Log files

```
$cd /srv/projectzomboid/server-data/Logs
```
## ADDING A MOD or ADJUSTING CONFIGS

```
$docker stop projectzomboid_project-zomboid_1
$vim /srv/projectzomboid/server-data/Server/aruezombi.ini
### Add Name of the mod at Mods= and the Steam ID of the mod at WorkshopItems= 
### Mods are separated with semicolon ;
$docker start projectzomboid_project-zomboid_1
```
