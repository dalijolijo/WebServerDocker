# WebServerDocker
Web server (to serve files) Docker image for personal purposes

## How To

Build the docker image:
```console
docker build -t webserver .
```

Spin up a container:

```console
docker run -d --rm --name webserver -p 80:80 -p 443:443 -v <FILE_DIR_ON_THE_HOST>:/var/www/<DOMAIN>/public_html webserver
```
