# Multiple Web Projects all-in-one Linux Server

## Overview
This is a template for deploying multiple projects with different domains or sub-domains all-in-one server. 
The major tools used in this setup are docker, docker-compose and nginx. Prometheus and Grafana have also been added for sever monitoring.

Follow the instruction in other section to use the template with ease.
### Project Setup

1. Create a sub-directory for each project which contains it's Dockerfile and docker-compose.yml file

2. Run ```docker-compose build``` in the root directory containing the root docker-compose.yml file to build all subproject.

    ****Proceed to step 3 only if step 2 is successful*
3. Run ```docker compose up -d``` to start your project in daemon mode.


### Build Individual Project

To build individual project 

1.  Run ```cd dirname``` to the project dir.

2. Run ```docker compose build``` to build the current docker project.

3. Run ```docker compose up -d``` to spin up the containers in daemon mode.