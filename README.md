Role Name
=========

Install and configure Zabbix plugin elastizabbix (https://github.com/mkhpalm/elastizabbix) for monitoring Elasticsearch Cluster

Installation
------------

erozario.elastizabbix is an Ansible role distributed globally using Ansible Galaxy. In order to install erozario.elastizabbix role you can use the following command.

    $ ansible-galaxy install erozario.elastizabbix
    
This only needs to be setup on one of the zabbix web interface

- Import the XML template (supports zabbix 2.4 and greater) files/templates_app_elasticsearch.xml
- Add node to the newly imported template

Requirements
------------

- Python 2/3 on an elastic node with zabbix agent installed

Role Variables
--------------
    ---

    elastizabbix_ttl: 10
    elastizabbix_url: localhost


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      become: yes
      roles:
        - role: erozario.ansible-role-elastizabbix
          elastizabbix_ttl: 15
          elastizabbix_url: elasticsearch.com.br

License
-------

MIT

Author Information
------------------

https://www.linkedin.com/in/eduardo-rozario/
