# cs-server
Dockerized LinuxGSM CS 1.6 Server with basic plugins

### Creating the server

The server should start after creating it.
```
docker run -d -p 27020:27015/udp -e START_MAP=fy_pool_day -e ADMIN_STEAM=0:1:1234566 -e SERVER_NAME="Sebi's server" --name cs cs1.6-server:alpha
```

In order to stop, start a stopped server or remove an existing server, use this commands respectively.

##### Stop
```
docker stop cs
```

##### Start
```
docker start cs
```

##### Remove

```
docker rm cs
```

### [Dockerhub](https://hub.docker.com/r/sebiglesias/cs1.6-server/) image
```
docker run -d -p 27020:27015/udp -e START_MAP=fy_pool_day -e ADMIN_STEAM=0:1:1234566 -e SERVER_NAME="Sebi's server" --name cs cs1.6-server:alpha +log
```

