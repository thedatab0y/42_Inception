
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


### NGINX

NGINX is a lightweight and fast web server that is used to serve static or dynamic web sites. In this project, I'm using NGINX to handle secure communication between your WordPress site and users using the TLSv1.2 security protocols.

### WordPress + php-fpm

WordPress is a popular web content management system that is used to create dynamic web sites. It's easy to use and has a large community of developers creating plugins and themes to add functionality and customize the look of your site.

### MariaDB

MariaDB is an open-source database management system that is compatible with MySQL. It's used to securely and efficiently store data. In this project, MariaDB is used to store your WordPress site's data.

## Prerequisites

To use this project, it is essential to have Docker and Docker Compose installed on the machine.
Docker is a popular platform that allows developers to build, ship, and run distributed applications in containers. Containers are lightweight, portable, and self-sufficient units of software that can be easily moved between different environments.

With Docker, you can package your application along with all its dependencies into a container, which can then be deployed to any machine that has Docker installed. This makes it easy to create consistent development, testing, and production environments, without having to worry about differences in underlying infrastructure.

