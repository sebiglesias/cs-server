# cs-server
Dockerized LinuxGSM CS 1.6 Server with basic plugins

### Creating the server

```
docker run -d -p 27020:27015/udp -e START_MAP=fy_pool_day -e ADMIN_STEAM=0:1:1234566 -e SERVER_NAME="Sebi's server" --name cs hlds:alpha
```
