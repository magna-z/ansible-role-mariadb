mariadb
---

Configure and run unprivileged vanila MariaDB as Docker container into systemd.service.


### Ссылки:
- <https://mariadb.org>
- <https://github.com/MariaDB>
- <https://hub.docker.com/_/mariadb/>


### Переменные:
- **`mariadb_root_password`** *(type=string, mandatory)* - MariaDB root user password.

- **`mariadb_docker_image`** *(type=string, default="mariadb:latest")* - Docker image for using into systemd.service.

- **`mariadb_docker_network`** *(type=string, default="bridge")* - Docker network used as `docker run --network=...`.
- **`mariadb_docker_publish_ports`** *(type=list, default=[])* - List of publish a container’s ports to the host as `docker run --publish=...`.

- **`mariadb_uid`** & **`mariadb_gid`** *(type=number, default=3306)* - System user and group for run MariaDB and store data as `docker run --user=...`.
