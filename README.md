= ElasticSearch / Heka / Kibana with a Consul cluster

This git repo is about how to set up and ElasticSearch Heka Kibana stack 
with service discovery, on consul.

The technologies that will be used in this learning tool are:

  - [Vagrant](https://www.vagrantup.com/)
  - [Ansible](http://www.ansible.com/home)
  - [Docker](https://www.docker.com/)
  - [ElasticSearch](https://www.elastic.co/products/elasticsearch)
  - [Heka](http://hekad.readthedocs.org/en/v0.9.2/)
  - [Kibana](https://www.elastic.co/products/kibana)

== Pre-requisities

  - Install [vagrant](https://www.vagrantup.com/downloads.html).
  - Run: vagrant box add chef/centos-7.0

== Consul setup

The **Consul** cluster will be running on Bare Centos 7 machines.

The configuration is all done in the [consul folder](consul/).

We will be creating 3 VMs to run the **consul cluster**, and those 
VMs will be setup using **Ansible**.

To spin up the cluster, just git clone the repo, go in the **consul/** folder
and run **vagrant up**.
