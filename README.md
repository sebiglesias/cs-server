# cs-server
Dockerized LinuxGSM + SteamCMD CS 1.6 Server with basic plugins

### Creating the server

#### Build the image

```
make build
```

The server should start after creating it.
```
docker run -d -p 27015:27015/tcp -p 27015:27015/udp -p 27020:27020/udp -p 27005:27005/udp -e START_MAP=fy_pool_day -e ADMIN_STEAM=0:1:1234566 -e SERVER_NAME="Sebi's server" --name cs cs1.6-server:alpha +log
```
In order to stop, start a stopped server or remove an existing server, use these commands respectively.

```
docker stop/start/remove cs
```

### [Dockerhub](https://hub.docker.com/r/sebiglesias/cs1.6-server/) image
```
docker run -d -p 27015:27015/tcp -p 27015:27015/udp -p 27020:27020/udp -p 27005:27005/udp -e START_MAP=fy_pool_day -e ADMIN_STEAM=0:1:1234566 -e SERVER_NAME="Sebi's server" --name cs cs1.6-server:alpha +log
```
