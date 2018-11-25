# Docker Compose template project for pgAdmin4 

Based on the [official Docker image](https://www.pgadmin.org/download/pgadmin-4-container/) from [Docker Hub](https://hub.docker.com/r/dpage/pgadmin4/).

## Initial setup

1. Clone this repo.
1. Create `.env` file from `.env.example`. Snippet: 
    ```bash
    cp .env.example .env
    ```
1. Edit `.env` file and set own values to the variables:
    * `PG_ADMIN_TAG` - tag of the image. `latest` is default value. For more info see [page of the image tags](https://hub.docker.com/r/dpage/pgadmin4/tags/).
    * `PG_ADMIN_PORT` - port binding. `5050` is default value.
    * `PGADMIN_DEFAULT_EMAIL` - initial account email. `user@domain.com` is default value.
    * `PGADMIN_DEFAULT_PASSWORD` - initial account password. `SuperSecret` is default value.
1. Up containers `docker-compose up`
