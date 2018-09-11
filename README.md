# simple-eureka

配置host
172.26.232.211 eureka-one
172.26.232.212 eureka-two 
172.26.232.213 eureka-three


启动实例
java -jar com.simple.eureka.jar --spring.application.name=eureka-one --server.port=8761 --eureka.client.service-url.defaultZone=http://eureka-one:8761/eureka/,http://eureka-two:8761/eureka/,http://eureka-three:8761/eureka/
java -jar com.simple.eureka.jar --spring.application.name=eureka-two --server.port=8761 --eureka.client.service-url.defaultZone=http://eureka-one:8761/eureka/,http://eureka-two:8761/eureka/,http://eureka-three:8761/eureka/
java -jar com.simple.eureka.jar --spring.application.name=eureka-three --server.port=8761 --eureka.client.service-url.defaultZone=http://eureka-one:8761/eureka/,http://eureka-two:8761/eureka/,http://eureka-three:8761/eureka/
