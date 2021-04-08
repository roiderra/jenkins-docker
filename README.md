# Jenkins docker
* Jenkins CI with docker client
* Check the docker group on your mashine with 
* cat /etc/group | grep docker
* ..and change in Dockerfile
* git clone https://github.com/roiderra/jenkins-docker
* docker build -t jenkins-docker .
* docker run -p 8080:8080 -p 50000:50000 -v /var/jenkins_home:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock --name jenkins -d jenkins-docker
