# kafka-actions

This [GitHub Action](https://github.com/features/actions) sets up Bitnami Kafka instance.

Docker images source [bitnami/kafka](https://hub.docker.com/r/bitnami/kafka).

---------
## Usage

See [action.yml](action.yml)

Basic:
```yaml
    - name: Start Kafka
      uses: 280780363/kafka-action@v1.0
      with:
        kafka version: "latest" # Optional, kafka version
        zookeeper version: "latest" # Optional, zookeeper version
        kafka port: 9092 # Optional, kafka port
        zookeeper port: 2181 # Optional, zookeeper port
        auto create topic: "true" # Optional, auto create kafka topic
```

Now you should be able to publish to Kafka broker running at `localhost:9092` 