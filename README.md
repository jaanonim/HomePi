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

Also it have setup for pi fan and automatic updates.

## Installation:

Create files form examples: `example.config.yaml` and `example.inventory.ini` as `config.yaml` and `inventory.ini`.

Run playbook (may need to install roles before):

    ansible-playbook ./main.yaml
