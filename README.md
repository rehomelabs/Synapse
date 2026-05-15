# Synapse

mkdir -p ~/matrix/synapse/data
cd ~/matrix
nano docker-compose.yaml
sudo docker compose run --rm synapse
sudo nano ~/matrix/synapse/data/homeserver.yaml
sudo docker compose down
rm docker-compose.yaml
nano .env
nano docker-compose.yaml
sudo docker compose up


open browser go to sub.yourdomain.com and check for matrix success page

sudo docker exec -it {synapse container name} /bin/bash

register_new_matrix_user -c /data/homeserver.yaml http://localhost:8008

open element web or element desktop client 
