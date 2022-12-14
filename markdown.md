# CIT352 FINAL PROJECT
# POSTGRESQL
## Install Postgresql and configure it to start on boot
```
$ sudo dnf install postgresql

$ systemctl enable postgresql
```
## How to check if it runs at boot
```
$ systemctl | grep postgresql
```
If it says "loaded active running," its already running.
# NODE
## Install and start app.js in Nodejs
```
$ npm install pm2 -g

$ pm2 start app.js
```

## To start Nodejs at boot
```
# Generate Startup Script
$ pm2 startup

# Freeze your process list across server restart
$ pm2 save

$ reboot
```
## To see is node apps (app.js) runs at boot
```
$ pm2 list
```
## To monitor Nodejs apps
```
$ pm2 monit
```
# Express
## Install Express

```
$ mkdir myapp
$ cd myapp

$ npm init
```
When this command prompts you for a bunch of the config settings, press enter (accepting the default) for all of them except for where the entry point says "index.js"
Change index.js to app.js
```
$ npm install express
```



## To check if it express is hosting a website
 - Go to Firefox
 - Enter "localhost:3000" in search bar



![image](C:\Users\garyg\Desktop\Fall 2022\Operating Systems 1\Screenshot (176).png)
