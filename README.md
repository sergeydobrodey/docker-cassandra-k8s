# Docker Cassandra K8s

Apache Cassandra docker image based on ubuntu-slim that is optimized to run on Kubernetes.

Note that this image is unstable and under development.

```
make build
docker run -d gcr.io/google_samples/cassandra:v12
docker run -ti --rm gcr.io/google_samples/cassandra:v12-DEV cqlsh CASSANDRA_IP
```
Production container: ubuntu slim + openjdk + cassandra - 241 MB
Developer container: ubuntu slim + openjdk + cassandra + python(cqlsh) - 263 MB
