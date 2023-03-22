[Overview (docker.com)](https://docs.docker.com/get-started/)
[Docker comes to Raspberry Pi - Raspberry Pi](https://www.raspberrypi.com/news/docker-comes-to-raspberry-pi/)

**Install:**
```bash
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
```

**Setup:**
```bash
sudo groupadd docker
sudo usermod -aG docker $USER
newgrp docker
docker run hello-world
```
