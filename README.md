# kafka
Compose Kafka without Zookeeper. The idea is prepared for a local development environment. The Kafka container is based on the `apache/kafka` image, which is a popular choice for running Kafka in Docker.

Note: SASL authentication is enabled.

# Prerequisites
- Docker: Make sure you have Docker installed on your machine. You can download it from [Docker's official website](https://www.docker.com/get-started).

# Usage
To use this Docker Compose file, follow these steps:
1. Clone this repository or download the `docker-compose.yml` file.
2. Open a terminal and navigate to the directory where the `docker-compose.yml` file is located.
3. Run the following command to start the Kafka container:
   ```bash
   docker-compose up -d
   ```
4. Wait for the Kafka container to start. You can check the logs using:
   ```bash
    docker logs kafka -f
    ```
5. Once the container is running, you can access AKHQ (Kafka UI) at `http://localhost:8091` and create topics, produce messages, and consume messages using the UI.
   