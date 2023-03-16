# Dotfiles

## Troubleshooting
- ansible -e NETNS_NAMESERVER=x.x.x.x -e NETNS_NAME=default-vpn  -e NETNS_CONF_FILE=wireguardconfig NETNS_IP=x.x.x.x/x --ask-become-pass netns.yml
