"How to Install and troubleshooting"
========================================

####References and DOCS:

* https://github.com/DemocracyOS/app/wiki/Installation
* https://github.com/DemocracyOS/app/wiki/Environment-variables
* https://github.com/DemocracyOS/app/wiki/Environments-and-config-files
* https://github.com/componentjs/guide/blob/master/component/getting-started.md#configuring-github-access
* [ clone me ] (https://github.com/DemocracyOS/docs.git) docs official

####To install DemocracyOS we need to follow the next three steps:

  * [ Fork me ] complete and contribute.
  
  * Install npm (node package manager)
    'apt-get install npm'

####Install NodeJS in debian/ubuntu
=================================
 ```
 add-apt-repository ppa:chris-lea/node.js  
 ```
 
####Install nvm (node version manager, for updates)
================================================
 
 ```
 apt-get install curl
 apt-get install nvm
 curl https://raw.githubusercontent.com/creationix/nvm/v0.11.1/install.sh | bash
 source ~/.profile
 nvm ls-remote
 
 #nvm install     <version>
 nvm install     v4.0.0
 node -v
 ```
####Install MongoDB in debian/ubuntu
=================================
 ```
 http://docs.mongodb.org/master/tutorial/install-mongodb-on-debian/mongodb
 apt-key adv --keyserver keyserver.ubuntu.com --recv 7F0CEB10
 echo "deb http://repo.mongodb.org/apt/debian wheezy/mongodb-org/3.0 main" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.0.list
 apt-get update
 apt-get install -y mongodb-org
 apt-get install -y mongodb-org=3.0.6 mongodb-org-server=3.0.6 mongodb-org-shell=3.0.6 mongodb-org-mongos=3.0.6 mongodb-org-tools=3.0.6
 service mongod start
 mongod --httpinterface
 ```
 
####Configure db space
===================
 ```
 mkdir -p /data/db
 chmod 0755 /data/db
 mongod --dbpath /data/db --port 27017
 ```
 
####Configure files and env variables
==================================
  
'Coming soon'

####Para que funque
=======================
Clonar el branch "1.0.0" del Democracy
git clone -b 1.0.0 https://github.com/DemocracyOS/app.git

con eso corre, teniendo todo las configuraciones anteriores
