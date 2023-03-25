# CI / CD Strategy with Docker

## Create Java APP Docker image
```bash
$ docker build -t scalian_training-java-hello-world:0.0.1 -f java_app/devops/dev.Dockerfile java_app
$ docker run -d --rm -p 8085:8080  --name java-app   scalian_training-java-hello-world:0.0.1
$ curl localhost:8085/hello
$ docker stop java-app
$ cd ..
```
