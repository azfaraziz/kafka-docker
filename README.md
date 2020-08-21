# Kafka Docker 

Simple Kafka setup the runs a single Zookeeper and Kafka Broker within Docker.

## Dependencies 
| Application | Version |
| --- | --- |
| docker | 19.03.5 |
| docker-compose | 1.24.1 |

Utilize `brew` to install any of these dependencies

## Installed Versions
These are the versions that are utilized within Docker
 
| Application | Version | Docker Tag |
| --- | --- | --- |
| Zookeeper | 3.4.9 | zookeeper:3.4.9 |
| Kafka | 2.2.1 | confluentinc/cp-kafka:5.2.2 |

## Utilization
This uses `docker-compose` for "managing" Kafka.

### Start
```bash
docker-compose up -d
```
Remove the `-d` if you want it to run in the foreground

### Stop
```bash
docker-compose down
```

### Access to Kafka
| Server | Host:Port |
| --- | --- |
| Bootstrap Server | localhost:9092 |
| Zookeeper | localhost:2181 |
