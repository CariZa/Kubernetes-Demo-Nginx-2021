# Kubernetes-Demo-Nginx-2021

A demo with using docker-compose and the kubernetes to run an nginx environment

## docker-compose

Run the docker-compose

    $ docker-compose up -d

View the website:

http://localhost:8000

I've pushed a publicly available image here (just for testing purposes):

https://hub.docker.com/repository/docker/cariza/nginxtest

## Kubernetes

Run on kubernetes cluster:

    $ kubectl apply -f ./k8s

Port forward service:

    $ kubectl port-forward service/nginx-service 8005:80
