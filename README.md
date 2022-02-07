# Dockerized qBittorrent that works only via VPN

# Features

- Easy installation and using
- OpenVPN with the killswitch
- When the VPN connection is lost the qBittorrent container restarts

## Configuration
Just save openvpn configuration file into ```openvpn_config``` directory with ```conf``` extension.
OpenVPN config must work without typing password

## Start 

```Shell
sudo bash up.sh
```
or
```Shell
sudo UID=${UID} GID=${GID} docker-compose up
```
Then go to http://localhost:8889/ (username: ```admin```, password: ```adminadmin```)

# Thanks to
- [Werner Beroux](https://github.com/wernight) for [Dockerized qBittorrent](https://github.com/wernight/docker-qbittorrent)
- [Wyatt Gill](https://github.com/wfg) for [OpenVPN Client for Docker](https://github.com/wfg/docker-openvpn-client)
- [Will Farrell](https://github.com/willfarrell) for [Docker Autoheal](https://github.com/willfarrell/docker-autoheal)
