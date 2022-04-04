# DevOpsTools

## Private docker registry
To enable the local Nexus 3 private docker registry, you should follow instructions in the website: https://www.ivankrizsan.se/2016/06/09/create-a-private-docker-registry/

And, you can create a new file /etc/docker/daemon.json 
with the contents
{ "insecure-registries":["host:port"] }

and then restart docker daemon by doing:

$ sudo service docker restart
