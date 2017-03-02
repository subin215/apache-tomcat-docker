# apache-tomcat-docker
---
## Description
Simple template for docker-compose to build images for an application deployed on a tomcat server where http is proxying requests to tomcat. Only port 80 on the apache container is exposed to the host.

---

## Instructions
- Place your .war file of your application inside the /tomcat folder
- Check all the settings and Dockerfiles to replace placeholders with your application names and contexts. 
- Run `docker-compose up -d` to create the docker images and deploy the containers.
