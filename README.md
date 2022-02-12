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

docker run --network semprini-blog-filekafkatransport_kafka-cluster --name foo 231b7a181c0f

docker cp in/Sample1000.csv foo:/Sample1000.csv
 