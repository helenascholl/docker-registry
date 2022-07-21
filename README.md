# Custom Docker registry

A custom Docker registry running behind a Traefik reverse proxy.

## Prerequisites

### `.env` file

Create an `.env` file based on `template.env` and add your hostname.

### Users

Add a comma-seperated list of `htpasswd` credentials to the `.env` file.

Create a user using the `htpasswd` command:

```shell
htpasswd -nbB user password
```

## Start the registry

```shell
docker-compose up -d
```
