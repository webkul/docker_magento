# docker_magento
Pull Image from DockerHub :-

docker pull webkul/magento:latest

Run your container by following command :-

"docker run -d -p 80:80 -p 3306:3306 webkul/magento:latest"

Note-: No other services should be running on port 80 and 3306 of your host system. If so, change ports in the above docker command.

In order to access the credentials of your database, you have to get the container's console. Run the following command-:

"docker ps" (to get the containers id)

after that run the command 

"docker logs container_id"

in that logs you will get the mysql username and password to connect with the database.
