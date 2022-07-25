# Homer

https://github.com/bastienwirtz/homer
================================
**mkdir homer**
```wrap
b4bz/homer:latest
```
```wrap
8082:8080
/www/assets
/home/jassa/homer

USER
GROUP

#environment:
#  - UID=1000
#  - GID=1000
```

**mkdir homer**
```wrap
docker run -d -p 8085:8080 -v /home/jassa/docker/homer/assets:/www/assets --name="homer" --restart=always b4bz/homer:latest
```
```wrap
sudo chmod 775 homer
sudo usermod -aG docker $USER

 newgrp docker
 sudo systemctl start docker
 sudo systemctl enable docker
 sudo systemctl status docker
```
```wrap
Getting Icons for your Dashboard
https://github.com/walkxhub/dashboard-icons
