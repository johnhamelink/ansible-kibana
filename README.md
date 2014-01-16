kibana ansible role
===================

[Kibana](http://www.elasticsearch.org/overview/kibana/) is a static frontend to
elasticsearch which allows you to monitor your data in realtime.

Requirements
------------

 - Ubuntu (13.04 or 13.10)

Role Variables
--------------

### Set the user ansible will log in with

    user: ubuntu

### Set the domain name kibana will resolve to - this is for the nginx configuration

    kibana_domain: log.example.com

### Set the url to retrieve kibana from

    kibana_url: https://github.com/elasticsearch/kibana/archive/master.zip

### Set the location of the elastic search database

    es_address: http://log.example.com/es/

Dependencies
------------

 - Nginx installed and runnning
 - Elasticsearch installed and running

Setup
-----

Generate a htpasswd file (You can use an online tool if you don't have apache
installed - [this one is known to work](http://www.htpasswdgenerator.net/)) and
put it in `roles/kibana/files/htpasswd`.

Author Information
------------------

Issues and more at: [https://github.com/johnhamelink/ansible-kibana](https://github.com/johnhamelink/ansible-kibana)
