# kafka-actions

This [GitHub Action](https://github.com/features/actions) sets up Bitnami Kafka instance.

---------
## Usage

See [action.yml](action.yml)

Basic:
```yaml
    - name: Start Bitname Kafka
      uses: 280780363/kafka-action@v1.0
      with:
        kafka version: "latest"
        zookeeper version: "latest"
        kafka port: 9092
        zookeeper port: 2181
        auto create topic: "true"
```

Now you should be able to publish to Kafka broker running at `localhost:9092` 