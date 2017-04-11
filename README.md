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
