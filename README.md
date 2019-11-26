
# go-kafka-avro-poc

A library provides consumer/producer to work with kafka, avro and schema registry

## Installation

```
$ go get github.com/wagner-aos/go-kafka-avro
```

### Usage

[Examples](./examples)


* Setup kafka, schema-registry
    ```
    docker-compose up -d
    ```
    
* Add test messages
    ```
    go run producer/main.go -n 10
    ```
    
* Run consumer
    ```
    go run consumer/main.go
    ```
    
### References

* Kafka [sarama](https://github.com/Shopify/sarama)
* Encodes and decodes Avro data [goavro](https://github.com/linkedin/goavro)
* Consumer group [sarama-cluster](https://github.com/bsm/sarama-cluster)
* [schema-registry](https://github.com/confluentinc/schema-registry)
