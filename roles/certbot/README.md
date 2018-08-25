## Certbot command examples

Obtain certificates by placing files in a webroot directory.

```bash
sudo certbot certonly \
    --webroot --staging --agree-tos --no-eff-email \
    -m admin@example.com \
    -w /usr/share/nginx/html -d monki.biz -d www.monki.biz
```

Once a certificate is revoked (or for other certificate management tasks), all of a certificate’s relevant files can be removed from the system with the delete subcommand:

```bash
certbot delete --cert-name monki.biz
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

```bash
sudo certbot certonly --standalone \
    -d loki.cepaitis.eu \
    -d aha.cepaitis.eu \
    -d cactus.cepaitis.eu \
    -d jenkins.cepaitis.eu \
    -d kaunas.cepaitis.eu
```
