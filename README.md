#### Dockerizing an Angular app

Login to Docker Hub

```zsh
$ docker login
```

create an Angular container

```zsh
$ docker build -t {yourDockerUsername}/angular-app:1.0.0 .
```

Test the Angular container by running it. It should be visible at localhost:8080

```zsh
$ docker run -p 8080:80 {yourDockerUsername}/angular-app:1.0.0
```

Push the container to your Docker Hub account repository

```zsh
$ docker push {yourDockerUsername}/angular-app:1.0.0
```
