# Teashop CDN

A simple Content Delivery Network server that serves assets, such as images, to other parts of Teashop environment.

## Technologies used
- [Nginx](https://www.nginx.com/) - http server
- [Docker](https://www.docker.com/) - containerization

## Usage

This service is a part of Teashop application environment. To see the details of setting up the entire environment, go to [Teashop Ops](https://github.com/lukaszslazyk/teashop-ops) repository.

### Docker container

To setup the CDN in docker container, first build the container image by running the following command in project directory:
```
docker build -t teashop_cdn .
```

Then to run the container:
```
docker run -p 8080:80 teashop_cdn
```

You can access served content at [http://localhost:8080](http://localhost:8080)

## Notes

- You can add new assets to be served by putting them in assets directory.
