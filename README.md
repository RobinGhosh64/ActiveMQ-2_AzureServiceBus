Migrating JMS code from Active Apache MQ to Azure Service Bus.

1) Add the spring jms service bus module into your project po..xml

    <!-- Azure Service Bus -->
	<dependency>
    	<groupId>com.azure.spring</groupId>
    	<artifactId>azure-spring-boot-starter-servicebus-jms</artifactId>
    	<version>3.14.0</version>
	</dependency> 
    
2) Add 2 new parameters in your application.properties file

	spring.jms.servicebus.connection-string=<Connection String>

	spring.jms.servicebus.pricing-tier=Premium

3) Use spring.jms.servicebus.enabled=[true/false] 
if you decide to switch at runtime between Service Bus or Active Apache MQ product usage.
	
robin.ghosh@microsoft.com 	
