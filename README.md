# A6s JNLP Slave Docker Image   

This is a custom JNLP Slave image that is based on jenkinsci/jnlp-slave one.

Additional tools that are installed:

- helm@2.9.1
- kubectl@1.10.3
- docker@18.03.1
- docker-compose@1.21.1
- node@8.11.3
- yarn@1.7.0
- a6s-railway@0.1.12

# How to publish docker image?

```bash
docker login

docker build -t apigeeks/a6s-jnlp-slave:1.0.6 .
docker push apigeeks/a6s-jnlp-slave:1.0.6
```