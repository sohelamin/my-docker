# My Docker Environment

## Included
    - php
    - nginx
    - mariadb
    - redis

## Usage
    // Up the containers
    docker-compose up -d
    // Down the containers
    docker-compose down
    
    // Shell into a container
    docker exec -it mydocker_app_1 bash
    
    // Get the IP Address of a contaner
    docker inspect mydocker_nginx_1 | grep \"IPAddress
    
## Extra hosts
```
    app:
        ...
        ...
        extra_hosts:
            - "mysite.dev:172.18.0.6"
```
