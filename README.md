# Jenkins slave image with kubectl

Based on the deprecated image at https://github.com/GoogleCloudPlatform/continuous-deployment-on-kubernetes/blob/master/jenkins/docker-slave-image/Dockerfile , this image provides a slave base image containing the newest kubectl. Kubectl is supposed to be downward compatible.

At the moment, the only available image is based on a Jenkins 2.62 slave, `jenkinsci/jnlp-slave:2.62`. Feel free to add slaves based on other image varieties.
