# confluent-docker

sudo docker-compose up -d

sudo docker-compose exec kafka kafka-topics --create --topic foo --partitions 1 --replication-factor 1 --if-not-exists --zookeeper localhost:2181

sudo docker-compose exec kafka kafka-topics --describe --topic foo --zookeeper localhost:2181

sudo docker-compose down

./bin/kafka-avro-console-consumer --topic test --zookeeper localhost:2181 --from-beginning

