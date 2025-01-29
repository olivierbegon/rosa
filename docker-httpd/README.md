oc new-app https://github.com/olivierbegon/rosa.git  --name newapp-docker-httpd --context-dir=newapp-docker-httpd --strategy=docker
oc expose service/newapp-docker-httpd

 oc delete all --selector app=newapp-docker-httpd