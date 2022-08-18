# oanhnn/example-nginx-proxy-auto-ssl

An example for setting auto proxy and auto setup SSL with NGINX

- [x] Using `ghcr.io/nginx-proxy/nginx-proxy:alpine` to auto proxy
- [x] Using `ghcr.io/nginx-proxy/acme-companion` to auto get SSL

<p align="center">
   <img src="https://github.com/evertramos/images/raw/master/webproxy.jpg" />
</p>

## Refs

- https://github.com/nginx-proxy/nginx-proxy
- https://github.com/nginx-proxy/acme-companion
- http://jasonwilder.com/blog/2014/03/25/automated-nginx-reverse-proxy-for-docker/

## Requirements

- Docker Engine 19.03.0+
- Docker Compose 1.27.0+ (Docker Compose Plugin)

## Usage

- Launch the `nginx-proxy` stack in detached mode with:
  
  ```bash
  $ docker compose up -d
  ```

- Create a service in `reverse-proxy` docker network like example service
  
  ```bash
  $ cd example-svc
  $ docker compose up -d
  ```

- Now your service was lauch and proxy with SSL.

## Contributing

All code contributions must go through a pull request and approved by a core developer before being merged. 
This is to ensure proper review of all the code.

Fork the project, create a feature branch, and send a pull request.

If you would like to help take a look at the [list of issues](https://github.com/oanhnn/example-nginx-proxy-auto-ssl/issues).

## License

This project is released under the MIT License.   
Copyright © 2022 [Oanh Nguyen](https://github.com/oanhnn)   
Please see [License File](https://github.com/oanhnn/example-nginx-proxy-auto-ssl/blob/master/LICENSE) for more information.
