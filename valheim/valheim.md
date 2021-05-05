# Valheim docker container

- Easy docker-compose valheim
- https://github.com/lloesche/valheim-server-docker


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
   ```

# TODO:
config valheim better

### Fast join on server

https://nodecraft.com/support/games/valheim/how-to-quickly-find-and-join-your-valheim-server