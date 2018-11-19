# Jenkins
To allow Docker based builds through a Docker running Jenkins Server (see https://github.com/jenkinsci/docker/issues/263#issuecomment-286843737).

## Jenkins
```
> docker run --rm -p 8080:8080 -p 4040:4040 -v /var/run/docker.sock:/var/run/docker.sock \
 -v $PWD/jenkins_home:/var/jenkins_home logimethods/jenkins
```

`logimethods/jenkins` comes in two different flavors:
- `logimethods/jenkins:latest` (latest version of Jenkins)
- `logimethods/jenkins:lts` (lts version of Jenkins)

## BlueOcean
```
> docker run --rm -p 8080:8080 -p 4040:4040 -v /var/run/docker.sock:/var/run/docker.sock \
 -v $PWD/blueocean_home:/var/jenkins_home logimethods/blueocean
```

`logimethods/blueocean` comes in two different flavors:
- `logimethods/blueocean:latest` (latest version of BlueOcean)
- `logimethods/blueocean:lts` (our own "lts" version of BlueOcean)

