# based on https://github.com/GoogleCloudPlatform/continuous-deployment-on-kubernetes/blob/master/jenkins/docker-slave-image/Dockerfile

FROM jenkinsci/jnlp-slave:2.62

USER root

RUN apt-get update -y && \
      apt-get install -y jq \
        libapparmor-dev \
        libseccomp-dev

RUN wget --quiet \
        https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl && \
      mv kubectl /usr/local/bin && \
      chmod u+x /usr/local/bin/kubectl
