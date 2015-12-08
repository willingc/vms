Docker Dev

1. Install 
    Docker
    docker-compose
    docker-machine

    (For Windows and mac, use Docker Toolbox)

2.  Check your docker install
    docker-compose --version
    docker-machine --version

3. Clone the GitHub vms repo
   git clone xxxxx

 4. Change directory to vms

 5. docker-machine create -d virtualbox dev;

 6. eval "$(docker-machine env dev)"

 7. docker-machine ls   To check that the dev is running

 8. docker-compose build

 9. docker-compose up -d

 10. docker-compose run web /usr/local/bin/python create_db.py

11. Go to URL returned by `docker-machine ip` in browser.

12. 


dockerizing-django = vms
    web = vms
        docker_django = vms
             static = vms/static **
             Dockerfile = ../Dockerfile **