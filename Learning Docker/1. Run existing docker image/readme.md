# Docker basics
## Check docker version on your PC
``docker --version``

## Run hello-world image
``docker run hello-world``

## Check if containers exites successfully

``docker ps -a``


# Runing Postgres and PgAdmin
## PostreSQL

``docker run postgres``

## PgAdmin

Pull image locally

``docker pull dpage/pgadmin4``
Run container
``
docker run -p 5050:80 \
    -e "PGADMIN_DEFAULT_EMAIL=user@domain.com" \
    -e "PGADMIN_DEFAULT_PASSWORD=SuperSecret" \
    -d dpage/pgadmin4
``

