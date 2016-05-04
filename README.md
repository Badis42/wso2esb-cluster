### ESB clustred deployment ###

Following instructions will help you to setup the deployment

 Execute 
 
 ``` docker login dockerhub.private.wso2.com ```
 
 ```docker-compose up```

This will setup 

* Mysql server (container) with esbdb
* SVN server and create svn repo
* ESB-Manager runs on its own in a container
* ESB-Worker runs on its own in a container and clustred with ESB-Manager node
* Nginx load Balancer container and add ESB enpoints

