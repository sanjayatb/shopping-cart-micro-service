# Projects
 Software Projects
1) Execute mvn clean install to build the project or start trough an IDE
2) Download and Run Active mq server (http://www.apache.org/dyn/closer.cgi?filename=/activemq/5.15.9/apache-activemq-5.15.9-bin.zip&action=download)
3) Run DataBaseService.java class
   http://localhost:8090/h2-console/
4) Use OrderService.java to post default messages. This service is for testing the functionality
   http://localhost:8080/publish/order1/123

###Note
Failure in database connection, will not acknowledge to the queue. So message will be in queue.
Only success scenario will ack.
In database service down and start again, will consume message which ever left with out human intervention.
