# oanhnn/example-nginx-proxy-auto-ssl

An example for setting auto proxy and auto setup SSL with NGINX

- [x] Using `jwilder/nginx-proxy:alpine` to auto proxy
- [x] Using `jrcs/letsencrypt-nginx-proxy-companion` to auto get SSL

## Refs

- https://github.com/jwilder/nginx-proxy
- https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion
- https://github.com/buchdag/letsencrypt-nginx-proxy-companion-compose

## Usage

- Launch the `nginx-proxy` stack in detached mode with:
  
  ```bash
  $ docker-compose up -d
  ```

- Create service in `nginx-proxy` docker network like example service
  
  ```bash
  $ cd example-svc
  $ docker-compose up -d
  ```

- Now your service was lauch and proxy with SSL.

## Contributing

All code contributions must go through a pull request and approved by a core developer before being merged. 
This is to ensure proper review of all the code.

Fork the project, create a feature branch, and send a pull request.

If you would like to help take a look at the [list of issues](https://github.com/oanhnn/example-nginx-proxy-auto-ssl/issues).

## License

This project is released under the MIT License.   
Copyright © 2019 [Oanh Nguyen](https://github.com/oanhnn)   
Please see [License File](https://github.com/oanhnn/example-nginx-proxy-auto-ssl/blob/master/LICENSE) for more information.
