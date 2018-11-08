# A6s JNLP Slave Docker Image   

This is a custom JNLP Slave image that is based on jenkinsci/jnlp-slave one.

Additional tools that are installed:

- helm@2.9.1
- kubectl@1.11.3
- kubeadm@1.11.3
- docker@18.06.1
- docker-compose@1.21.1
- node@10.13.0
- yarn@1.10.1
- a6s-railway@0.1.15

# Volumes:

To make docker use host docker daemon:
- /var/run/docker.sock:/var/run/docker.sock
- /usr/bin/docker:/usr/bin/docker

To increase docker storage:
- /var/lib/docker

# How to publish docker image?

```bash
docker login

docker build -t apigeeks/a6s-jnlp-slave:1.0.11 .
docker push apigeeks/a6s-jnlp-slave:1.0.11
```