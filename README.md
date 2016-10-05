# Ansible Role: Elasticsearch ELK stack

[![Build Status](https://travis-ci.org/bakhti/ansible-elk.svg?branch=master)](https://travis-ci.org/bakhti/ansible-elk) [![Ansible Galaxy](http://img.shields.io/badge/galaxy-bakhti.elk-660198.svg)](https://galaxy.ansible.com/list#/roles/1243)

Setup [Elasticsearch ELK Stack](http://www.elasticsearch.org/overview/) on Debian/Ubuntu linux servers.
New [Kibana (v4)](https://github.com/elasticsearch/kibana) is installed by this role. Please check [kibana3](https://github.com/bakhti/ansible-elk/tree/kibana3) branch if you need to setup ELK with [previous](https://github.com/elasticsearch/kibana/tree/kibana3) version of Kibana.

## Vagrant Usage

### Install full elk stack:
    
    vagrant up

At the end of the provisioning log the ip is displayed
Log into the Kibana UI going to
    
    http://<>:5601/

### Install other components:

Use the appropiate tags in the vagrant file
- elk the default stask
- dash the filebeat dashboards
- logstash local logstash instance


## License

MIT

## Author Information

This role was created in 2014 by [Bakhti Aripov](http://bakhti.github.io/).
