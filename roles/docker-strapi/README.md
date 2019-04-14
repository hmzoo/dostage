docker-minio Ansible role
============================

Installs and configures the official [Docker minio] container.


Requirements
------------

You will need to configure a reverse proxy for HTTPS with basic auth.

Role Variables
--------------

```yaml
# Directory for storing pushed images on registry host.
docker_minio_data_directory: /opt/minio

# Port to expose to host machine, for use in reverse proxy.
docker_minio_expose_port: 9000
```

Dependencies
------------

  * Docker container support (e.g. marklee77.docker)
  * HTTPS reverse proxy (e.g. jdauphant.nginx)
