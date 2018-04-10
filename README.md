# Jenkins slave image with kubectl
[![Docker Stars](https://img.shields.io/docker/stars/appuio/jenkins-slave-k8s.svg)](https://hub.docker.com/r/appuio/jenkins-slave-k8s/)
[![Docker Pulls](https://img.shields.io/docker/pulls/appuio/jenkins-slave-k8s.svg)](https://hub.docker.com/r/appuio/jenkins-slave-k8s/)
[![Docker Automated build](https://img.shields.io/docker/automated/appuio/jenkins-slave-k8s.svg)](https://hub.docker.com/r/appuio/jenkins-slave-k8s/)

Different kubectl and Jenkins slave versions are available in the specific directories or tags.

Kubectl is installed by [Google Cloud Platform SDK](https://cloud.google.com/sdk/)
See [release notes](https://cloud.google.com/sdk/docs/release-notes) for more information.

## kubectl tags and versions
At the moment, the available image is based on [jenkinsci/jnlp-slave:2.62](https://hub.docker.com/r/jenkinsci/jnlp-slave/)
with [kubectl 1.8.6](https://kubernetes.io/docs/reference/kubectl/overview/)

| Folder | Jenkins slave | kubectl |
| --- | --- | --- |
| [jnlp_2](jnlp_2) | jenkinsci/jnlp-slave:2.62 | 1.8.6 |

Feel free to add slaves based on other image varieties.

## notes
Based on the deprecated image at [continuous-deployment-on-kubernetes](https://github.com/GoogleCloudPlatform/continuous-deployment-on-kubernetes/blob/master/jenkins/docker-slave-image/Dockerfile).
This image provides a slave base image containing the newest kubectl.
