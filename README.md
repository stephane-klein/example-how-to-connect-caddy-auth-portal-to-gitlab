# Example how to connect caddy-auth-portal to self hosted GitLab instance

How to connect [caddy-auth-portal](https://github.com/greenpau/caddy-auth-portal) to self hosted GitLab instance.

## Build stephaneklein/caddy-auth-portal:2.2.1-alpine Docker image

See [./docker-image/](./docker-image/)

I use [`hosts`](https://github.com/xwmx/hosts) to configure my local hostname:

```sh
sudo hosts add 127.0.0.1 example.com
```

Set variable env in [`docker-compose.yml`](docker-compose.yml)

```sh
docker-compose up -d
```

```sh
$ curl http://example.com
<h1>Hello world</h1>
```
