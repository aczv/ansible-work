# TODO

Install firewall on servers

```bash
sudo ufw allow 'OpenSSH'
```

## TODO

web
WAN faz
NAT 80, 443 to 24.41
nginx alias /.well-known to /var/.well-known
docker volume /var/certbot/.well-known:/var/.well-known
nginx ssl
certbot webroot
certbot renew

### Generate certificates

```bash
sudo certbot certonly --standalone \
    -d loki.cepaitis.eu \
    -d aha.cepaitis.eu \
    -d cactus.cepaitis.eu \
    -d jenkins.cepaitis.eu \
    -d kaunas.cepaitis.eu

sudo certbot certonly --standalone \
  -d zulu.cepaitis.eu \
  -d jenkins.cepaitis.eu \
  -d registry.cepaitis.eu \
  -d portainer.cepaitis.eu \
  -d smm.cepaitis.eu \
  -d smm-test.cepaitis.eu
```

## Renew certbot certificates

To non-interactively renew *all* of your certificates, run

    certbot renew

# TODO

## Install nginx on zulu

https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-16-04

