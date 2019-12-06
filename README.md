# eriks-project

## Requisites ( used during the implementation and tests):
- Software
  - ansible 2.9.2 or later
  - Vagrant 2.2.6 or later
  - Virtualbox 6.0 or later

- Hardware
  - 2 VCPUs
  - 4Gb of Ram

# Running:
## To run the project
  $ vagrant up
  $ cd ansible
  $ ansible-playbook -v site.yml

## To test Mariadb
  $ mysql -u [user] -h 192.168.56.11 -p

# Jenkins
## To create a simple jenkins server to test DSL
  $ cd ansible
  $ ansible-playbook -v common.yml
  $ ansible-playbook -v jenkins-deployment.yml

## To access Jenkins
http://192.168.56.11:8080/

