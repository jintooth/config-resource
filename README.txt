- Configuration Server
name: config
port: ${CONFIG_SERVER_PORT}
password: ${CONFIG_SERVER_PASSWORD}

- Eureka Server
name: eureka
port: ${EUREKA_SERVER_PORT}

Note: ${} is OS environment, please set or export firstly.


Eureka
http://localhost:8001/

ON Gateway
http://localhost:8002/users/chris
http://localhost:8002/usermgmt-service/chris

On Comsumer Demo
http://localhost:9100/chris

On Usermgmt Service
http://localhost:9004/chris

Hystrix Dashboard On Gateway
http://localhost:8002/hystrix/monitor?stream=http%3A%2F%2Flocalhost%3A8002%2Fhystrix.stream&title=All

Hystrix Dashboard On Monitoring (Hystrix Dashboard + Turbine)
http://localhost:8003/hystrix/monitor?stream=http%3A%2F%2Flocalhost%3A8003%2Fturbine.stream&title=Service