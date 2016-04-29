# jenkins-slave-docker

The Dockerfile and the supervisord.conf file combo allows one to create a CentOS based Jenkins slave Docker container. This container can be created on demand by Jenkins using the Docker plugin https://wiki.jenkins-ci.org/display/JENKINS/Docker+Plugin and a Docker registry that is hosting this Docker image.

The idea and content of this project is based on a blogpost by Paul Gier. https://developer.jboss.org/people/pgier/blog/2014/06/30/on-demand-jenkins-slaves-using-docker

#How to create the Jenkins slave Docker image and container?
1. Clone this repo
2. Build the Docker image using: docker build -t centos-jenkins-slave .
3. Create a container using: docker run -d centos-jenkins-slave
4. Verify that the container is running: docker ps
