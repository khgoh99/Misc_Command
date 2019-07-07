Nextcloud + Only Office + Traefik
---------------------------------

Follow setup instruction according to link below,

    https://medium.com/onlyoffice/deploying-onlyoffice-with-nextcloud-using-docker-compose-4a93387cc681
 
Go into the docker directory and replace the docker-compose.yml file and download rest of the file in the this directory.
Edit the db.env, traefik.env accordingly and create acme.json in location below,

    mkdir -p app/traefik
    touch app/traefik/acme.json
    chmod 600 app/traefik/acme.json
    
exec link below to start the server

    . traefik.env
    docker-compose up -d
    
    
