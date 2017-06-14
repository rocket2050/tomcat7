# Ansible Role: Tomcat 7

[![Build Status](https://travis-ci.org/devops/ansible-role-tomcat7.svg?branch=master)](https://travis-ci.org/devops/ansible-role-tomcat7)

An Ansible Role that installs Tomcat 7 on RedHat/CentOS Linux servers.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

* `tomcat7_packages:`
    ```
      - tomcat
      - tomcat-admin-webapps
      - tomcat-webapps
    ```
    Tomcat services installed the packages, Production environment recommended only use tomcat.


* `tomcat7_hostname: 192.168.33.10`
* `tomcat7_server_port: 8005`
* `tomcat7_catalina_port: 8080`
* `tomcat7_catalina_redirect_port: 8443`
* `tomcat7_ajp_port: 8009`
* `tomcat7_uriencoding: ""`

## Dependencies

None.

## Example Playbook

    - hosts: tomcat_hosts
      roles:
        - { role: "ansible-role-tomcat7" }

## License

 BSD

## Author Information
www.opstree.com
blog.opstree.com
