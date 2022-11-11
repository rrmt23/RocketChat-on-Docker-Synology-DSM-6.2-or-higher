# RocketChat-on-Docker-Synology-DSM-6.2-or-higher

If your CPU support AVX or AVX2 use mongo:5, if no use mongo:4.4. Firewall on DSM - IS OFF (!) or use rules for Docker containet subnet after installation.

Create folders in DSM for ex. volume1: /volume1/docker/mongodb/db /volume1/docker/mongodb/dump /volume1/docker/rocketchat/uploads /volume1/docker/rocketchat/emoji /volume1/docker/rocketchat/sounds

Open Portainer - Add Stack

Use code on Docker Compose

Deploy

Wait 5 min and open https://localhost:3111 or https://chat.domain.com

Use revers proxy on DSM: https://chat.domain.com (442 port for https) to localhost:3111 (80 port) and include WebSocket.

Check accessess folder on DSM for /docker/rocketchat/uploads if allow File uploads if allow File storage type -> File system.
