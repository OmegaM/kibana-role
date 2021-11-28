Role Name
=========

This role used for installing and configuring [Kibana](https://www.elastic.co/kibana)

Requirements
------------

	Modules: 
		- get_.url
		- yum
		- templates
	OS:
		- CentOS

Role Variables
--------------

|Variable name| Description | Default |
|-------------|-------------|---------|
| elk_stack_version | Version of ELK stack(Kibana, Elasticsearch, Logstash) | "7.15.2"|

Dependencies
------------

Role have no dependensies

Example Playbook
----------------
    - name: "Install and configure Kibana"
      hosts: kibana_hosts
      roles:
        - kibana
