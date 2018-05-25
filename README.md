# mcit_baremetal_pipeline

## Version 0.1.0

## Description

A pipeline to deploy openstack on a physical system

## Features

- the pipeline runs on jenkins
- Provisioning is done through ansible
- Updates the OS and configures the kernel for use, including nested virtualization
- Deploys and configures docker-ce and kubernetes
- Deploys Openstack using Kolla-Kubernetes in an AIO configuration

## Requirements

1. Deploys on CentOS/RHEL systems
2. The deployment is intended for physical servers, not virtual.
3. Uses a forked version of Kolla-Kubernetes, which can be found [here](https://github.com/jonathanelbailey/kolla-kubernetes).
4. The pipeline runs on jenkins.  A portable vagrant box running jenkins can be found [here](https://github.com/jonathanelbailey/mcit-jenkins).
5. While this is open for anyone to use, This is by no means a finished product and there are environment-specific configurations that may likely cause configuration issues.

## NOTICE

Expect this repo to change drastically since the method of deployment include physical infrastructure as well as virtual infrastructure.  Eventually that may get split out.  This was a POC made in just a few days, but work on this project will continue to persist.
