# SRT-Server for Docker

### OLD, USE https://github.com/AlexanderWagnerDev/srtla-server-docker INSTEAD OFF SRT-SEVRER-DOCKER

For all systems: docker run -d --name srt-server --restart always -p 8181:8181/tcp -p 8282:8282/udp alexanderwagnerdev/srt-server:latest

## Usage:

Stream-URL: srt://ip:8282/publish/live/{stream}

Watch-URL: srt://ip:8282/publish/live/{stream}

Stats-URL: http://ip:8181/stats

{stream} is your streamkey, that can be anything

## Build Docker Image self:

wget https://raw.githubusercontent.com/AlexanderWagnerDev/srt-server-docker/main/Dockerfile

Build Image: docker build --no-cache -t srt-server .

Run Container: docker run -d --name srt-server --restart always -p 8181:8181/tcp -p 8282:8282/udp srt-server

Docker Hub: https://hub.docker.com/r/alexanderwagnerdev/srt-server
