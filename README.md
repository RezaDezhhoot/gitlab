# Get started

## Gitlab interface

### Set environments
````bash
cp .env.example .env
````
### Launching gitlab on Docker
````bash
docker-compose up -d
````

### Retrieve the GitLab password with the following command.
````bash
docker exec -it gitlab-ce grep 'Password:' /etc/gitlab/initial_root_password
````
Now the gitlab is available with the username ****root**** on ****server-ip:8080****

## Gitlab runner
````bash
docker container exec -it gitlab-runner bash
````
### Inside container
````bash
 gitlab-runner register
````