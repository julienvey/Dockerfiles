FROM ubuntu

RUN apt-get update
RUN apt-get install -y git redis-server git-core curl openssh-server openjdk-6-jdk git curl maven wget

RUN wget -q -O - http://pkg.jenkins-ci.org/debian/jenkins-ci.org.key | apt-key add -
RUN sh -c 'echo deb http://pkg.jenkins-ci.org/debian binary/ > /etc/apt/sources.list.d/jenkins.list'
RUN apt-get update
RUN apt-get install -y jenkins