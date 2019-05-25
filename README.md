# ELK-FileBeat
Run ELK Stack On Ducker With Docker Compose 

# ElasticSearch+Filebeat+Kibana
You can run single node elasticsearch + Filebeat + kibana using files that inside this folder
In this folder we have : 
1- A docker compose file which our nodes will run with this file , you can run this file using following command : 

# sudo docker-compose -f docker-compose.yml up -d

you can see node status using following command : 

sudo docker ps

also you can remove all containers using following command :

sudo docker container rm -f $(sudo docker ps -aq)

2- logfile folder which contain an static log file (apache log) for indexing process

3- filebeat which we have filebeat.yml inside that.

# ElasticSearch+Filebeat+Kibana+Cluster
You can run 4 node elasticsearch + Filebeat + kibana using files that inside this folder. nodes are inside a cluster and can see each other inside the network.
In this folder we have : 
1- A docker compose file which our nodes will run with this file , you can run this file using following command : 

sudo docker-compose -f docker-compose.yml up -d

you can see node status using following command : 

sudo docker ps

also you can remove all containers using following command :

sudo docker container rm -f $(sudo docker ps -aq)

2- logfile folder which contain an static log file (apache log) for indexing process

3- filebeat which we have filebeat.yml inside that.

# ElasticSearch+Filebeat+Kibana+2Cluster
You can run 4 node elasticsearch + Filebeat + kibana using files that inside this folder. 2 nodes are inside a cluster and other nodes are inside another cluster. each cluster's node can see other nodes inside the cluster in the network.
In this folder we have : 
1- A docker compose file which our nodes will run with this file , you can run this file using following command : 

> sudo docker-compose -f docker-compose.yml up -d

you can see node status using following command : 

sudo docker ps

also you can remove all containers using following command :

sudo docker container rm -f $(sudo docker ps -aq)

2- logfile folder which contain an static log file (apache log) for indexing process

3- filebeat which we have filebeat.yml inside that.

