# Docker
## Commands used to create containers on docker:-
### Pull Images:
```
docker pull hello-world
```
```
docker pull nginx
```
```
docker pull httpd
```
### See Images:
```
docker images
```
### List of Containers:
```
docker ps
```
### Port Forwarding:
```
docker run -d -p 80:80 --name httpd-apache httpd
```
```
docker run -d -p 80:80 --name httpd-nginx httpd
```
### Stop Container:
```
Docker stop nginx
```
```
Docker stop apache
```
### Remove Container:
```
Docker rm nginx
```
```
Docker rm apache
```
### Kill Container:
```
docker kill nginx
```
```
docker kill apache
```
