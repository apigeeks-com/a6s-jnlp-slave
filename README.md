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

# Volumes:

To make docker use host docker daemon:
- /var/run/docker.sock:/var/run/docker.sock
- /usr/bin/docker:/usr/bin/docker

To increase docker storage:
- /var/lib/docker

# How to publish docker image?

Git tag and everything else CircleCI will do for you.