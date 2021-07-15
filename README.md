Stack for monitoring in docker service

For first run you should use this man:

git clone
For native start/stop actions you should use command:

docker-compose up -d  start stack
docker-compose stop   stop stack

For comfort use you should use command:

make docker-up    start stack
make docker-down  stop stack

For another functions read Makefile and run by analogy with the previous commands.

Grafana: http://ip_address:3000
Node-Red: http://ip_address:1880
Influxdb:

Don't forget include in service:
npm install node-red-contrib-wirenboard
################################################

How to install docker-compose

sudo curl -L "https://github.com/docker/compose/releases/download/1.26.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

sudo chmod +x /usr/local/bin/docker-compose