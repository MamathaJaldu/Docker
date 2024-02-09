  commands:
****docker ps  –    running containers
****docker ps -a – all hidden containers
****docker images – it showing images
****docker pull nginx – it pulls image nginx
****docker create nginx – it will create image
****docker start nginx – it will start nginx
****docker run nginx – it is like pull+create+start – it will pull image and create the image and run as container
****docker run -d  nginx   – it run image in detach mode and run in background
****docker run -d -p 8080:80 nginx – it runs in detach mode and 8080 is host port and 80 is docker image nginx port. Host port can be change but nginx 80 port will not change
****docker run -d -p 8080:80 nginx  --name some-nginx   - it will run with name and port with detach mode
****docker  rm <container id>  - it only remove stopped containers
****docker rm  -f <container id> - it will remove container without stopping
****docker rmi  <image id>  - it removes images
****docker rmi  `****docker images -a -q`  -  it removes all the images
