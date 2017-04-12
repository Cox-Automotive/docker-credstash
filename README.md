# Credstash Docker Container

Location on Docker Hub [`coxauto/credstash`](https://hub.docker.com/r/coxauto/credstash/)

A container for running [Credstash](https://github.com/fugue/credstash).

## Examples

```
docker run -i \
    -e AWS_ACCESS_KEY_ID=$AWS_ACCESS_KEY_ID \
    -e AWS_SECRET_ACCESS_KEY=$AWS_SECRET_ACCESS_KEY \
    -e AWS_SESSION_TOKEN=$AWS_SESSION_TOKEN \
    coxauto/credstash credstash setup
```

```
docker run -i \
    -v ~/.aws:/home/root/.aws \
    coxauto/credstash credstash setup
```