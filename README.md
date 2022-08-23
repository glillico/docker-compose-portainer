# portainer

A docker-compose file for my portainer environment.

## Usage 

### Starting

```bash
cd ~/portainer       # change to the portainer directory
docker-compose pull  # pulls the latest image
```

```bash
docker-compose up  # starts container
```

Once up and running, using a web browser go to http://dockerhost:9443 and login.

### Stopping

```bash
cd ~/portainer       # change to the portainer directory
docker-compose down  # stops the container
```

### Updating

```bash
cd ~/portainer          # change to the portainer directory
docker-compose pull     # pulls the latest image
docker-compose up -d    # restarts the container with the newer images
docker system prune -a  # deletes any unused images
```

### Uninstall

```bash
cd ~/portainer          # change to the portainer directory
docker-compose down -v  # stops the container and deletes the data volumes
docker system prune -a  # deletes any unused container images
```

## License

MIT

## Author Information

This project was created in 2022 by Graham Lillico.
