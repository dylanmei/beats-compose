beats-compose
-------------

Compose a simple `filebeats` -> `kafka` -> `logstash` -> `elasticsearch` pipeline.

# starting

```
docker-compose up
```

# using

write message via stdin

```
echo "hello" | docker run --rm -i --net beatscompose_default ryane/kafkacat -P -b kafka:9092 -t hello-messages
```
