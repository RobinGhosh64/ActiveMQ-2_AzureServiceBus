Migrate from Active Apache MQ to Azure Service Bus.

1) Add the spring jms service bus
2) Add 2 parameters in application.properties
spring.jms.servicebus.connection-string=<Connection String>
spring.jms.servicebus.pricing-tier=Premium
Switch from Active MQ to Azure Service Bus by runtime attribute with spring.jms.servicebus.enabled=false

Switch from Azure Service Bus to Apache Active MQ with spring.jms.servicebus.enabled=true
