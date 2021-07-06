# Confluent Certified Administrator for Apache Kafka Certification Examination 
1. Kafka fundamentals 15 % 
https://www.udemy.com/course/apache-kafka/

2. Managing, configuring, and optimizing a cluster for performance 30 %
https://www.udemy.com/course/kafka-cluster-setup/
3. Kafka Security 15 %
https://www.udemy.com/course/apache-kafka-security/learn/lecture/9437688?start=0#overview

4. Designing, troubleshooting, and integrating systems 40 %
https://www.udemy.com/course/kafka-monitoring-and-operations/

5. Mock test
https://www.udemy.com/course/confluent-certified-operator-for-apache-kafka-practice-test/learn/quiz/4895388#overview

# Slids
https://courses.datacumulus.com/downloads/kafka-beginners-bu5/

# Installation
```
brew install kafka
```
## Producer with keys
```
kafka-console-producer --broker-list 127.0.0.1:9092 --topic first_topic --property parse.key=true --property key.separator=,
> key,value
> another key,another value
```
## Consumer with keys
```
kafka-console-consumer --bootstrap-server 127.0.0.1:9092 --topic first_topic --from-beginning --property print.key=true --property key.separator=,

```
# Conduktor - Kafka GUI
Kafka does not come bundled with a UI, but Stephane Maarek have created a software name Conduktor to help you use Kafka visually.
You can download Conduktor here: https://www.conduktor.io/

# KafkaCat as a replacement for Kafka CLI
KafkaCat (https://github.com/edenhill/kafkacat) is an open-source alternative to using the Kafka CLI, created by Magnus Edenhill.
