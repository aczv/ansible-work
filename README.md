# ansible-work

Ansible playbooks to provision developer machine.

## Prepare controll machine

Install Ansible:

    https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html

Install common tools:

    sudo apt-get install git mc

## Prepare target machines

Install OpenSSH Server:

    sudo apt install openssh-server

Copy SSH keys to remote machines, e.g.:

    ssh-copy-id localhost

Run add-hoc command on all servers:

    ansible all -a "uname -a"

## certbot

Your certificate and chain have been saved at:

    /etc/letsencrypt/live/zulu.cepaitis.eu/fullchain.pem

Your key file has been saved at:

    /etc/letsencrypt/live/zulu.cepaitis.eu/privkey.pem

### Certbot command examples

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
