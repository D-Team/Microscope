#Microscope

##Meteor's site
[Q42 Meteor Learning](https://github.com/Q42/Meteor-Learning)
[Q42 How to deploy Meteor on Google Compute Engenie](http://q42.com/blog/post/98968122208/how-to-deploy-meteor-on-google-compute-engine)


##How to install Meteor and Meteorite on Ubuntu
###Update and upgrade your Ubuntu
Depending on how up-to-date your image is, this may take a while.
`sudo apt-get update && sudo apt-get upgrade`
###Install CURL
`sudo apt-get install curl`
###Install Node.JS
####Getting Required Stuff
Here we get all the required dependencies.
```
sudo apt-get update
sudo apt-get install build-essential -y
sudo apt-get install git -y
sudo apt-get install python libssl-dev -y
```
####Install Node.js from GitHub Clone
```
cd /usr/local/src
sudo git clone git://github.com/joyent/node.git
user@ubuntu:/usr/local/src/node$ sudo ./configure
user@ubuntu:/usr/local/src/node$ sudo make
```
This will take a while.
`user@ubuntu:/usr/local/src/node$ sudo make install`
####Upgrading Node.js via GitHub Clone
```
cd /usr/local/src/node
sudo git checkout master
sudo git pull origin master
sudo git checkout vx.x.x
sudo ./configure
sudo make
sudo make install
```
###Install meteor
`curl https://install.meteor.com | sh`
###Install meteorite
`sudo -H npm install -g meteorite`
