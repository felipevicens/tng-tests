build:
	docker build -t easyglobalmarket/mqtt-probe:v2.0 .
push:
	docker push easyglobalmarket/mqtt-probe:v2.0	
run:
	docker run  -e "IP=$(ip)" -e "PORT=$(port)" -e "CLIENTS=$(clients)" -e "COUNT=$(count)" -e "SIZE=$(size)" -e "USERNAME=$(username)" -e "PASSWORD=$(password)" --name docker-mqtt-probe --net=egm easyglobalmarket/mqtt-probe
stop:
	docker stop docker-mqtt-probe
	docker rm docker-mqtt-probe
