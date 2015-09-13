"How to Install and troubleshooting"
========================================

####References and DOCS:

* https://github.com/DemocracyOS/app/wiki/Installation
* https://github.com/DemocracyOS/app/wiki/Environment-variables
* https://github.com/DemocracyOS/app/wiki/Environments-and-config-files
* https://github.com/componentjs/guide/blob/master/component/getting-started.md#configuring-github-access
* [ clone me ] https://github.com/DemocracyOS/docs.git

##To install DemocracyOS we need to follow the next three steps:

  * [ Fork me ] complete and contribute.
  
  * Install npm (node package manager)
    'apt-get install npm'

##Install NodeJS in debian/ubuntu
=================================
  'sudo add-apt-repository ppa:chris-lea/node.js  
   curl https://raw.githubusercontent.com/creationix/nvm/v0.11.1/install.sh | bash
   sudo apt-get install curl
  '

##Install nvm (node version manager, for updates)
================================================
   'sudo apt-get install nvm
   curl https://raw.githubusercontent.com/creationix/nvm/v0.11.1/install.sh | bash
   source ~/.profile
   nvm ls-remote
   
   #nvm install     <version>
   nvm install     v4.0.0
   node -v
  '
##Install MongoDB in debian/ubuntu
=================================
http://docs.mongodb.org/master/tutorial/install-mongodb-on-debian/
mongodb
  
    apt-key adv --keyserver keyserver.ubuntu.com --recv 7F0CEB10
    echo "deb http://repo.mongodb.org/apt/debian wheezy/mongodb-org/3.0 main" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.0.list
    apt-get update
    apt-get install -y mongodb-org
    apt-get install -y mongodb-org=3.0.6 mongodb-org-server=3.0.6 mongodb-org-shell=3.0.6 mongodb-org-mongos=3.0.6 mongodb-org-tools=3.0.6
    service mongod start
    mongod --httpinterface
  
##Configure db space
===================
  
    mkdir -p /data/db
    chmod 0755 /data/db
    mongod --dbpath /data/db --port 27017
  
##Configure files and env variables
==================================
  
  ######Coming soon








