# E-commerce (MSA Architecture)

## Server List
 - SpringCloudEureka : https://github.com/GreedTy/SpringEurekaService
 - SpringCloudGateway : https://github.com/GreedTy/SpringCloudGateway
 - SpringCloudConfig & SpringCloudConfig(yml) : https://github.com/GreedTy/SpringCloudConfigServer & https://github.com/GreedTy/spring-cloud-config
 - SpringCloudMicroServices : https://github.com/GreedTy/SpringCloudServices (User, Order, Catalog)

## 기술스텍
 - App : SpringBoot 2.6.3 / Java JDK 11(G1GC)
   - Dependency : SpringEureka&Eureka-client, SpringGateway, SpringConfig-Server&Config, OpenFeign, Resilience4j, SpringSleuth, Actuator, JPA, Security, JWT
 - Middleware : Kafka&Kafka-connect(user, order, catalog Data Sync), RabbitMQ(SpringCloudBus(config.yml push용도), 
 - Monitoring : Prometheus, Grafana, Zipkin
 - Database : MariaDB, H2

## Eureka
<img width="1326" alt="스크린샷 2022-02-01 오후 12 30 19" src="https://user-images.githubusercontent.com/35190067/151914270-fc6c5b78-b986-491b-bbed-cb2c279f924a.png">

## Kafka(3.1.0 version & curl download / topic PostmanCanary call post connector & JSON body request)
<img width="1313" alt="스크린샷 2022-02-01 오후 12 28 35" src="https://user-images.githubusercontent.com/35190067/151914308-85c26037-c46b-4842-96b1-289c4a095157.png">

## Zipkin
<img width="1325" alt="스크린샷 2022-02-01 오후 12 26 14" src="https://user-images.githubusercontent.com/35190067/151914345-67c5c784-0033-48cd-b570-73ff79d697af.png">
<img width="1329" alt="스크린샷 2022-02-01 오후 12 24 38" src="https://user-images.githubusercontent.com/35190067/151914350-ab0c5a84-bc17-4912-8136-16bb5f77333b.png">

## Prometheus&Grafana(apigateway, user, order, catalog service monitoring)
<img width="1312" alt="스크린샷 2022-02-01 오후 12 25 53" src="https://user-images.githubusercontent.com/35190067/151914368-3ed7cf5e-42e8-4ebe-be3c-708fea038ffa.png">
<img width="1333" alt="스크린샷 2022-02-01 오후 12 25 31" src="https://user-images.githubusercontent.com/35190067/151914371-e9ba139c-5e0d-4f18-9dab-4c6f3c2f2031.png">
