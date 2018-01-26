# [Jenkins image from](https://github.com/jenkinsci/docker)

This is a mirror from Oficial Jenkins

# Docker Run Command
```docker run -u="jenkins:jenkins" -d --restart "always" -p 8080:8080 -p 50000:50000 --name jenkins -v /home/jenkins/jenkins/:/var/jenkins_home -v /etc/localtime:/etc/localtime:ro -e JAVA_OPTS=-Duser.timezone=America/Argentina/Buenos_Aires jenkins```
