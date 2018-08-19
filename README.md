# Ansible Utilities

Ansible Utilities is a collection of useful playbook that I use for my projects, and also in mi company every day.
I try to group the playbooks by functionality.

# Backups

  - pb-wordpress-data.yml - This playbook create zip files with all the data of my blogs and store them in S3
  - pb-mysql-docker-data.yml - Create a mysql-dump of the database inside a docker and the send it to S3 bucket
  - pb-mysql-docker-data.yml - Create a zip file with the folder that you have as volume in docker containers and send 
  them to S3 bucket
  
  
# How to use this project

You need to create a virtual environment, install the requirements.txt with pip. And after that you have to create a 
vars folder like the example with your own data.

Also in the credentials folder you have to put all files like pem files in order to connect to the machine, this pem 
files a referenced in the group_vars/wordpresss.yml file.