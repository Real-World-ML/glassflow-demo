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
             : Install Clickhouse operator (Helmfile)
             : Install Clickhouse instance (Kustomization)
    section .NET Core
        2016 - 2017 
             : .NET Core 1.0
             : .NET Core 1.1
             : .NET Framework 4.6.2
             : .NET Core 2.0
             : .NET Framework 4.7
             : .NET Framework 4.7.1
        2018 - 2019 
             : .NET Core 2.1
             : .NET Core 2.2
             : .NET Framework 4.7.2             
             : .NET Core 3.0
             : .NET Core 3.1
             : .NET Framework 4.8
    section Modern .NET
        2020 : .NET 5
        2021 : .NET 6
        2022 : .NET 7
             : .NET Framework 4.8.1
```

## 1. Clickhouse


### 1.1 clickhouse-operator


https://github.com/Altinity/clickhouse-operator/blob/master/docs/operator_installation_details.md



### 2.1  clickhouse-instance