# Template for hosting multiple project in a server using docker

Project Setup

1. Create a subdirectory for each project which contains it's Dockerfile and docker-compose.yml file

2. Run ```docker-compose build``` to build your subproject.

    Proceed to step 3 only if step 2 is successful.
3. Run ```docker compose up -d``` to start your project in daemon mode.


Build Individual Project

To build individual project 

cd into the project dir

run docker compose build