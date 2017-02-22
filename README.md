[![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Build Status](https://travis-ci.org/grycap/ansible-role-kafka.svg?branch=master)](https://travis-ci.org/grycap/ansible-role-kafka)

Apache Kafka Role
===================

Install Apache Kafka (Only working for Ubuntu 16)

Role Variables
--------------

The variables that can be passed to this role and a brief description about them are as follows.

	base_kafka_version: "0.10.1.1"
	kafka_version: "2.12-{{ base_kafka_version }}"

Example Playbook
----------------
```
- hosts: server
  roles:
  - { role: 'grycap.kafka' }
```

Contributing to the role
========================
In order to keep the code clean, pushing changes to the master branch has been disabled. If you want to contribute, you have to create a branch, upload your changes and then create a pull request.  
Thanks
