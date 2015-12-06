#Tanaguru Ansible Role
This Ansible role will install the` Tanaguru Opensource Accessibility` on Ubuntu 12.04/14.04 LTS.
Before using this role, you can modify the variables or if you wish, you can continue with the defaults that has been provided with the role.
``` yaml
---
tanguru_debian_pkgs:
  - openjdk-7-jre
  - unzip
  - libmysql-java
  - mysql-server
  - python-mysqldb
  - tomcat7 
  - libspring-instrument-java
  - xvfb
  - mailutils
  - postfix

locale: 'en_US.UTF-8'

tanaguru_download_link: "http://download.tanaguru.org/Tanaguru/tanaguru-3.1.0.i386.tar.gz"

fixfox_esr_link: "http://download-origin.cdn.mozilla.net/pub/firefox/releases/24.0esr/linux-x86_64/en-US/firefox-24.0esr.tar.bz2"

tanaguru_parameters:
  db_name: 'tgdatabase'
  db_user: 'tguser'
  db_password: 'tgPassword'
  url: 'http://localhost:8080/tanaguru/'
  admin_email: 'admin@example.com'
  admin_passwd: 'tanaguru15'
```
 - If you want to read about the prerequisites of Tanaguru on Ubuntu, please follow this [link](http://www.tanaguru.org/en/content/ubuntu-prerequisites-tanaguru-3x)
  - [Here](http://www.tanaguru.org/en/content/ubuntu-installation-tanaguru-3x) is the official installation procedure on Tanagure website.

Hope this role will help you. Thanks!
