# eriks-project

## Requisites ( used during the implementation and tests):
- Software
  - ansible 2.9.2 or later
  - Vagrant 2.2.6 or later
  - Virtualbox 6.0 or later
  - Vault password as a file

- Hardware
  - 2 VCPUs
  - 4Gb of Ram

# Running:

## Create vault password as a file
  $ cat <<EOF > /tmp/vault-cred                                            
f56817f28d      
EOF

## To run the project (This will run both MariaDB and Jenkins as a containers)
  $ vagrant up
  $ cd ansible
  $ ansible-playbook -v site.yml

## To test Mariadb
  $ mysql -u [user] -h 192.168.56.11 -p

## To access Jenkins and run the DSL job already imported
http://192.168.56.11:8080/

## The JOB DSL is in the Jenkinsfile
