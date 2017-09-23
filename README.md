# docker-template

A minimal and secure [Alpine Linux][alpine] based [Docker][docker] image.

## Configuration

### Host user mapping

Host user and group can be mapped to a container by defining `HOST_UID` and
`HOST_GID` environment variables. If the variables are left undefined the
container will execute its command as `nobody:nobody`.

### Default gateway

Container's default gateway can be changed by defining a `CONTAINER_GATEWAY`
environment variable. Its value can be either an IP address or a hostname.
For to be able to change the gateway the container needs to have `NET_ADMIN`
capabilities.

## License

This project is licensed under the MIT License.

[alpine]: https://alpinelinux.org/
[docker]: https://www.docker.com/
