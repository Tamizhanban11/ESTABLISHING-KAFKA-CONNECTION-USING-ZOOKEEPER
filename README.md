# Kafka Setup and Execution Guide

## Step 1: Install Kafka and Zookeeper
1. Download Kafka from [Apache Kafka](https://kafka.apache.org/downloads).
2. Extract the files to a folder on your system.

## Step 2: Start Zookeeper
1. Open a terminal/command prompt.
2. Navigate to the Kafka directory and run:
    ```bash
    bin/zookeeper-server-start.sh config/zookeeper.properties
    ```

## Step 3: Start Kafka Broker
1. Open another terminal/command prompt.
2. Navigate to the Kafka directory and run:
    ```bash
    bin/kafka-server-start.sh config/server.properties
    ```

## Step 4: Create a Kafka Topic
1. Run the following command to create a topic named "test-topic":
    ```bash
    bin/kafka-topics.sh --create --topic test-topic --bootstrap-server localhost:9092 --partitions 1 --replication-factor 1
    ```

## Step 5: Verify Kafka Topic Creation
1. To list Kafka topics, run:
    ```bash
    bin/kafka-topics.sh --list --bootstrap-server localhost:9092
    ```

---
