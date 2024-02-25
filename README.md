# Home Pi

My setup for my home raspberry pi server.

## Contains:

- portainer - for managing containers
- grafana - for cool graphs
- pihole - for ad block and as dns
- nginx - for reverse proxy to be able to refer to services by domain names
- ims - for my custom "smart home system"
- vpn - for access from outside network
- monitoring - for monitoring pi performance and temperature
- internet - for monitoring internet speed

Also it have setup for pi fan and automatic updates.

## Installation:

Create files form examples: `example.config.yaml` and `example.inventory.ini` as `config.yaml` and `inventory.ini`.

Generate ssl certificates for nginx:

    openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout ./ssl/cert.key -out ./ssl/cert.crt

And put passphrase to certificates to `cert.pass` file.

Run playbook (may need to install roles before):

    ansible-playbook ./main.yaml
