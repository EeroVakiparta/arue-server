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

# Valheim sucks a lot of cache so it should be rebooted daily


  512  docker ps
  513  cd /etc/
  514  ls -l
  515  vim cron.daily
  516  crontab -e
 // to restart every day at 5am
  0 5 * * * docker restart e4051da78849

  517  htop
  518  docker ps
  519  htop
