# Runs 
```
sudo docker run -d   -p 34197:34197/udp   -p 27015:27015/tcp   -v /opt/factorio:/factorio   --name factorio   --restart=always   factoriotools/factorio
```

# logs
```
docker logs factorio
```


# update
```
docker stop factorio
docker rm factorio
docker pull factoriotools/factorio
```
# TODO:

- Make into docker-compose

https://github.com/factoriotools/factorio-docker

