This repository provides an image for Nginx on Raspberry Pi.
Automated builds currently fail since Docker Hub currently doesn't support ARM platforms.

### Environment Variables
If the environment variable ```NGINX_NO_UPDATE``` is present,  then Nginx will not be updated prior to starting it, as this  saves startup time if necessary. 
```
docker run --rm -it -e NGINX_NO_UPDATE= ckulka/rpi-nginx
```
Updating Nginx before running it is, however, the default setting.
 
### docker-compose
A sample ```docker-compose.yml``` file can be found in the git repo: https://github.com/ckulka/rpi-nginx

Forked from https://github.com/ckulka/rpi-nginx
