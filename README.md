### ESB clustred deployment ###

Following instructions will help you to setup the deployment

 Execute 
 
 ``` docker login dockerhub.private.wso2.com ```
 
 ```docker-compose up```

This will setup 

* A mysql server (container) with esbdb
* ESB-Manager runs on its own in a container
* ESB-Worker runs on its own in a container and clustred with ESB-Manager node

