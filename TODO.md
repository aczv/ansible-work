# TODO

## Install firewall on servers

```bash
sudo ufw allow 'OpenSSH'
```

## Install nginx on zulu

https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-16-04

## Generate certificates

```bash
sudo certbot certonly --standalone \
    -d loki.cepaitis.eu \
    -d aha.cepaitis.eu \
    -d cactus.cepaitis.eu \
    -d kaunas.cepaitis.eu
```

## Renew certbot certificates

To non-interactively renew *all* of your certificates, run

    certbot renew

## molecule

https://molecule.readthedocs.io/en/latest/installation.html

## deve/servers

- sudo apt install tree

- docker compose

- Chef InSpec

## axios config

veikiantis konfigas ant bob:

```
    axios: {
      baseURL: 'http://127.0.0.1:3001/api',
      browserBaseURL: 'https://aha.cepaitis.eu/api'
      // prefix: '/api'
      // baseURL: '/api'
    },

    proxy: [
      //['/api', {
        //target: process.env.BACKEND_URL || 'http://127.0.0.1:3030'
      //}]
    ],
```
