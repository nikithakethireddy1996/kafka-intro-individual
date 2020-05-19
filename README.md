# kafka-intro-individual

## kafka commands used:
- In order to start the zookeeper service we use the command
```
.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
```
- In order to start the kafka service we use the command
```
.\bin\windows\kafka-server-start.bat .\config\server.properties
```
- In order to create a unique topic we use the command
```
.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic tik-tok
```
- In order to list all created topics we use the command
```
.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list
```
- In order to start a Kafka producer for writing messages to your unique topic we use the command
```
.\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic tik-tok
```
- In order to start a Kafka consumer for retrieving messages from your unique topic we use the command
```
.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic tik-tok --from-beginning
```
