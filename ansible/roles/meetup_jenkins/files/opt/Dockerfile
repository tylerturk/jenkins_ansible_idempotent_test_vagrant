FROM ubuntu
MAINTAINER Dennis Rowe

RUN apt-get update
RUN apt-get -y install software-properties-common
RUN apt-add-repository ppa:ansible/ansible
RUN apt-get update
RUN apt-get -y install ansible
RUN apt-get -y install rubygems-integration
RUN gem install serverspec
RUN gem install rake

