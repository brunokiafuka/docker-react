`docker build -f <file name> .` - set a custom docker file

### Docker volume

> volumes allow us to map files in our local machine with files in a container.

`docker run -p 3000:3000 [-v /app/node_modules] [-v $(pwd):/app] <image id>`

`pwd` - present working dir

`[-v /app/node_modules]` - bookmarking a file

docker run -p 3000:3000 -v \$(pwd):/app brunokiafuka/frontend

`docker run -it brunokiafuka/frontend yarn test` - running test

# Nginx

### Build phase | run phase

> **84** is important. 80 is the default port for nginx

`docker run -p 8080:80 <image id>`
