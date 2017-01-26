# Docker Nginx-Proxy
nginx-proxy sets up a container running nginx and [docker-gen][1].
docker-gen generates reverse proxy configs for nginx and reloads nginx when containers are started and stopped.
Please see [upstream docs](https://github.com/jwilder/nginx-proxy) for more information.

## Improvments by this fork

- Using supervisor as process manager
- More clean workspace
- Some nginx tuneups by default
- Proper IP & Protocol passing to backends
- ...

## `VIRTUAL_UPSTREAM`
This Env variable can be added so that you can define your custom backends. (it should be full url like `http://my_app`)  
This is very useful specially when we are using nginx-proxy in a swarm cluster.
