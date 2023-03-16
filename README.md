# Dotfiles

## Examples 
### Create VPN network namespace
```
ansible -e NETNS_NAMESERVER=x.x.x.x -e NETNS_NAME=default-vpn  -e NETNS_CONF_FILE=wireguardconfig NETNS_IP=x.x.x.x/x --ask-become-pass netns.yml
sudo systemctl start netns-default-vpn
sudo ip netns exec vpn su $USER $(/usr/bin/flatpak run org.mozilla.firefox) # Runs firefox flatpak in vpn container
```

## Troubleshooting
- ERROR! couldn't resolve module/action 'flatpak' => ansible-galaxy collection install community.general

