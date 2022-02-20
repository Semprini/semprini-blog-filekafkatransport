# semprini-blog-filekafkatransport
Code for a blog post

Kafka:

docker-compose up -d

Producer:

docker build .

> ...

> Successfully built 231b7a181c0f

docker network ls

> 2cf58f114f20   semprini-blog-filekafkatransport_kafka-cluster   bridge    local

docker run -d --network semprini-blog-filekafkatransport_kafka-cluster --name foo f374580e2e5d

docker cp in/Sample1000.csv foo:/Sample1000.csv
