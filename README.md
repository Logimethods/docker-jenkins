# jenkins
To allow Docker based builds through a Docker running Jenkins Server

```
> docker run --rm -p 8080:8080 -p 4040:4040 -v /var/run/docker.sock:/var/run/docker.sock -v $PWD/jenkins_home:/var/jenkins_home logimethods/jenkins
```

For BlueOcean, have a look at [logimethods/blueocean](https://github.com/Logimethods/docker-blueocean)