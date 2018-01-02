# IMPORTANT
Whenever you run by first time, you must reload the nginx configuration files.
This can ve achieved by typing:
docker exec -it container_name service nginx reload
* Where container_name is the name of the nginx container
=======
# odoo-nginx-reverse-proxy
Odoo instance with docker. Odoo customized with workers and a nginx container that acts as a reverse proxy.
