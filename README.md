# Jenkins Example
## Jenkins Install
### Docker Pull

```shell
docker pull jenkins/jenkins:lts
```

### Docker Run

```shell
docker run -it --name jenkins -p 8080:8080 -p 50000:50000 -d -v /var/run/docker/sock:/var/run/docker.sock -v jenkins_home:/var/jenkins_home -u root jenkins/jenkins:lts
```

### Docker Container In

```shell
docker exec jenkins bash
```

## Jenkins Init
### Password
```shell
cd /var/jenkins_home/secrets/initialAdminPassword
```