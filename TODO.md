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

