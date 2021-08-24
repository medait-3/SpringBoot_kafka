 download kafka
 cd to folder

 run
 ./bin/zookeeper-server-start.sh config/zookeeper.properties
 
 bin/kafka-server-start.sh config/server.properties 
 go postman 
 http://localhost:8080/api/kafka  =>post
 {
    "field1":"field1",
    "field2":"field2"
}
 http://localhost:8080/api/kafka/v2 =>post
 {
    "title":"hello",
    "description":"you"
}
 show in console
  bin/kafka-console-producer.sh --topic quickstart-events --bootstrap-server localhost:9092
