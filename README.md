# springboot-kafka
SpringBoot Kafka Example

docker exec -it kafka-dev_kafka_1 kafka-topics --bootstrap-server localhost:29092 --topic springboot-kafka --create --partitions 1 --replication-factor 1

docker exec -it kafka-dev_kafka_1 kafka-console-consumer --bootstrap-server localhost:29092 --topic springboot-kafka --from-beginning

docker exec -it kafka-dev_kafka_1 kafka-console-producer --broker-list localhost:29092 --topic springboot-kafka 
> Hello from the terminal
