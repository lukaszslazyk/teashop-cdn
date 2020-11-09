# Teashop CDN

A simple Content Delivery Network server that serves assets, such as images, to other parts of Teashop environment.

## Technologies used
- [Nginx](https://www.nginx.com/) - www server
- [Docker](https://www.docker.com/) - containerization

## Usage

To setup the CDN on docker container, first build the container image by running the following command in project directory:

```
docker build -t teashop_cdn .
```

Then to run the container:

```
docker run -p 8080:80 teashop_cdn
```

You can access served content at [http://localhost:8080](http://localhost:8080)
