FROM jenkins/jenkins:lts
ENV JAVA_OPTS -Djenkins.install.runSetupWizard=false
RUN /usr/local/bin/install-plugins.sh job-dsl workflow-aggregator git
USER root
RUN apt-get update && apt-get install -y python-pip
EXPOSE 8080
USER jenkins

