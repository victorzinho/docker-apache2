# docker-apache2
Basic Apache2 on top of official [debian:jessie](https://hub.docker.com/_/debian/) image.

## Running

Run detached, exposing port 80 and mounting a custom `sites-enabled` directory:

```
docker run -d -p 80:80 -v /path/to/sites-enabled:/etc/apache2/sites-enabled --name=apache2 apache2
```

Get a [minimal sites-enabled directory](https://github.com/victorzinho/docker-apache2/tree/master/sites-enabled) to start with.