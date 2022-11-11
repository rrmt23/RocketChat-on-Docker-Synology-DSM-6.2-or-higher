# RocketChat-on-Docker-Synology-DSM-6.2-or-higher

If your CPU support AVX or AVX2 use - mongo:5 if no support AVS use - mongo:4.4. 
Firewall on DSM - IS OFF (!) or use rules for Docker containet subnet after installation RocketChat.

Step: 1
Create folders in DSM for ex. volume1: 
/volume1/docker/mongodb/db /volume1/docker/mongodb/dump 
/volume1/docker/rocketchat/uploads 
/volume1/docker/rocketchat/emoji 
/volume1/docker/rocketchat/sounds

Step 2:
Open Portainer or Docker Compose - Add Stack

Step 3:
Use code on Docker-Compose.yaml

Step 4:
Deploy

Step 5:
Wait 5 min and open https://localhost:3111 or https://chat.domain.com

FYY:
1) Use revers proxy on DSM: https://chat.domain.com (442 port for https) to localhost:3111 (80 port) and include WebSocket.

2) Check accessess folder on DSM for /docker/rocketchat/uploads if allow File uploads if allow File storage type -> File system.
