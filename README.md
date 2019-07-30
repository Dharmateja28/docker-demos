### redis
    Running simple redis server on docker using prebuilt docker image

    To just build redis server docker image use below command

        sudo docker build -t dharmatejat/redis:latest .

    To run docker container run below command

        sudo docker run dharmatejat/redis:latest

    To run and interact with our docker container running below command

        sudo docker run -it dharmatejat/redis:latest sh

### node-test
    Running simple node web app on docker using prebuilt node image

    To just build simple node web docker image use below command

        sudo docker build -t dharmatejat/node-test:latest .

    To just build redis server using docker use below command here we use port mapping to access a port on docker container from our machine

        sudo docker run -p 8080:8080 dharmatejat/node-test

### visits
    Count visits to website here we need both redis and node-web(can be multiple) which will on different dockers but still they should interact with each here we start using docker compose(docker-compose.yml)

    To build and run docker containers

    docker-compose up --build

    To just run docker containers

    docker-compose up

    To stop all the containers

    docker-compose down

### frontend_react_app
    Using volumes where we use references to files instead of directly copying them.
