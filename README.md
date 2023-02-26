# mysql_in_docker
```
docker pull mysql/mysql-server:latest
``
```
docker run -d -p 3306:3306 --name mysql-docker-container -e MYSQL_ROOT_PASSWORD=sergey -e MYSQL_DATABASE=photo_app -e MYSQL_USER=sergey -e MYSQL_PASSWORD=sergey mysql/mysql-server:latest
``
```
sudo docker exec -it mysql-docker-container bash
```
```
mysql -u root -p
```
##  you will enter the password which you had set when running the docker run command. In our case, the password of the root user is set to sergey.
```
SELECT user FROM mysql.user;
```
```
show databases;
```
