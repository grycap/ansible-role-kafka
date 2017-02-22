[![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Build Status](https://travis-ci.org/grycap/ansible-role-kafka.svg?branch=master)](https://travis-ci.org/grycap/ansible-role-kafka)

Apache Kafka Role
===================

Install [Apache Kafka](https://kafka.apache.org/).  
This role has been tested only with Ubuntu 16. Is not ensured that it will work with other systems.

Role Variables
--------------

Variables used in this role:

	# Install info
	base_kafka_version: "0.10.1.1"
	kafka_version: "2.12-{{ base_kafka_version }}"
	## System info
	kafka_system_user_name: kafka
	kafka_system_group_name: kafka
	kafka_system_comment: Kafka system user
	kafka_system_shell: /bin/false
	kafka_system_user_home: "/var/lib/{{ kafka_system_user_name }}"

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
