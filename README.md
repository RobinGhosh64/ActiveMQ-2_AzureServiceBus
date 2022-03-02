Migrate from Active Apache MQ to Azure Service Bus.

1) Add the spring jms service bus module into your projec2

    <!-- Azure Service Bus -->
		<dependency>
    		<groupId>com.azure.spring</groupId>
    		<artifactId>azure-spring-boot-starter-servicebus-jms</artifactId>
    		<version>3.14.0</version>
		</dependency> 
    
2) Add 2 parameters in application.properties
spring.jms.servicebus.connection-string=<Connection String>
spring.jms.servicebus.pricing-tier=Premium

  3)
Switch from Active MQ to Azure Service Bus using another  runtime attribute with spring.jms.servicebus.enabled=true

Switch from Azure Service Bus to Apache Active MQ with spring.jms.servicebus.enabled=false
