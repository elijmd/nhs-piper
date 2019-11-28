# NHS-PIPER
This project contains two apps:  
* mongo_sender 
* solr_sender  

Both apps read data from a Kafka pipe fed by scrapy-nhs and send it to mongo and solr.
Each app is launched via the start_piper.sh script wich takes a piper type as a parameter i.e mongo or solr.
The solr,mongo hosts and port, sleep delay used to wait for zookeeper and kafka to be up and running are env variables.
