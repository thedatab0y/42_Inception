# Inception

<div style="display" align="center">
<img src="./rscs/docker.png" width='42%'>
</div>

This project from 42 school aims to broaden your knowledge of system administration by using Docker.

## Mandatory part

Each Docker image must have the same name as its corresponding service.
Each service has to run in a dedicated container:
  You then have to set up:
  - A Docker container that contains NGINX with TLSv1.2 or TLSv1.3 only.
  - A Docker container that contains WordPress + php-fpm (it must be installed and configured) only without nginx.
  - A Docker container that contains MariaDB only without nginx.
  - A volume that contains your WordPress database.
  - A second volume that contains your WordPress website files.
  - A docker-network that establishes the connection between your containers.
  - Your containers have to restart in case of a crash.

Here is an example diagram of the expected result:

<img width="562" alt="photo" src="https://user-images.githubusercontent.com/54292953/147146268-a616f39a-3f16-41f8-80c9-db5494c3dfe7.png">
