FROM jenkinsci/blueocean:1.0.0-b24

USER root
#RUN apt-get -qq update \
#   && apt-get -qq -y install \
#   curl

RUN curl -sSL https://get.docker.com/ | sh

RUN usermod -a -G staff jenkins

USER jenkins
