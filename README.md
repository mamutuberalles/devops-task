# Formlabs DevOps home assignment

This repository contains a home assignment code for DevOps applicants for Formlabs.

See all open jobs at https://careers.formlabs.com/


## Task

0. Fork this repo.
1. Create a deployable docker image for the application.
    - Feel free to switch up technologies. For example you can use `buildah` instead of Docker.
2. Create a Kubernetes deployment and service for the application.
    - Just aim for the simplest setup, no ingress deployment is needed. Feel free to use Helm.
    - You can use [Minikube](https://minikube.sigs.k8s.io/docs/start/) or [k3s](https://k3s.io/) or any other Kubernetes distribution you are familiar with.
3. Create automation to build, test and deploy the application when a change happens in git.
    - Feel free to switch up technologies. For example you can use an Ansible playbook or a Jenkins pipeline.
4. Send us the fork where you did your work.

### Notes

- Explain as much as possible in the commit message(s) and/or comments if needed. See more on commit messages [here](https://chris.beams.io/posts/git-commit/).
- It would be great if you'd also write about why you choose a certain technology if there are alternatives to consider.


From me:

See the issues, where I've documented the progress, and executive decisions of the tasks.
Also, the commits are detailed as much as could be.


I chose docker because that is the one I have years of experience working with.
Docker also has built in k8s cluster which is handy when deploying an application is part of the testing process.
I've used helm because I have years of experience working with it, so no extra added difficulty, and looks better/cleaner.
I've used github actions since it was an obvious choice, I've worked with bitbucket pipelines and azure pipelines, both would've needed extra setup, and learning github actions was worth working with.
