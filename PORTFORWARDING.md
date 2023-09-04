# PULL IMAGES 
```bash
 docker pull hello-world
```
```bash
 docker pull nginx
```
```bash
docker pull ubuntu/apache2
```
# SEE IMGAGES/INSPECT
```bash
 docker images
```
```bash
 docker inspect
```
# PORT FORWADING 
```bash
docker run --name mynginxl -p 80:80 -d nginx
```
```bash
docker run --name myapache -p 80:80 -d ubuntu/apache2
```
# KILLING IMAGE
```bash
docker kill mynginxl
```

