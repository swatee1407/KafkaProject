# KafkaProject
The producer in this case uses "localhost:9092" boostrap server for kafka.

Follow below steps and consume messages over kafka topic.
1. Start the zookeeper server: 
C:\kafka_2.12-2.5.0\bin\windows>zookeeper-server-start.bat ../../config/zookeeper.properties

2. Start the kafka server
C:\kafka_2.12-2.5.0\bin\windows> kafka-server-start.sh ../../config/server.properties

3. Start the consumer to listen on localhost:9092
C:\kafka_2.12-2.5.0\bin\windows>kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic first_topic

4. Run the java class ProducerDemo from your intellij or any other IDE.
5. Verify the message send "hello-world" in this case.

C:\kafka_2.12-2.5.0\bin\windows>kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic first_topic
hello-world

