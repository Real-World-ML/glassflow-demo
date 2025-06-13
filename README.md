---

Use the timeline chart to see the actions to be taken 

```mermaid

timeline
    title Boostrap steps

    section Infra components
        1. Kafka
             : 1.1 Install Strimzi Kafka operator (Helmfile)
             : 2.2 Install Strimzi Kafka instance (Kustomization)
        2. Clickhouse
             : 2.1 Install Clickhouse operator (Helmfile)
             : 2.2 Install Clickhouse instance (Kustomization)
        3. NATS
             : 3.1 Install NATS (Helmfile)

     section Glassflow
        2016 - 2017
             : .NET Core 1.0
             : .NET Core 1.1
             : .NET Framework 4.6.2
             : .NET Core 2.0
             : .NET Framework 4.7
             : .NET Framework 4.7.1
    
    section K8S Jobs
        2020 : .NET 5
        2021 : .NET 6
        2022 : .NET 7
             : .NET Framework 4.8.3
```

---

## 1. Kafka
    
### 1.1 Strimzi Kafka operator
  
### 1.2  Strimzi Kafka instance

### 1.3 Misc

```
bin/kafka-topics.sh bin/kafka-topics.sh --bootstrap-server kafka-9d65-kafka-brokers.strimzi.svc.cluster.local:9092 --create --topic users --partitions 1 --replication-factor 1
```

Created topic users.

```
echo '{"event_id": "123", "user_id": "456", "name": "John Doe", "email": "john@example.com", "created_at": "2024-03-20T10:00:00Z"}' | bin/kafka-console-producer.sh --bootstrap-server kafka-9d65-kafka-brokers.strimzi.svc.cluster.local:9092 --topic users
```

```
bin/kafka-console-consumer.sh --bootstrap-server kafka-9d65-kafka-brokers.strimzi.svc.cluster.local:9092 --topic user_events_with_duplicates
```

---

## 2. Clickhouse
  
### 2.1 clickhouse-operator
    
https://github.com/Altinity/clickhouse-operator/blob/master/docs/operator_installation_details.md
  
### 2.2  clickhouse-instance

### 2.3 Misc

```sh

clickhouse-chi-4782.clickhouse.svc.cluster.local

```

---

## 3. NATS
    
### 3.1 NATS installation


---

## Tools
- [Helmfile](https://github.com/helmfile/helmfile)

