# IMPORTANT
Whenever you run by first time, you must reload the nginx configuration files.
This can ve achieved by typing:
docker exec -it container_name service nginx reload
* Where container_name is the name of the nginx container
=============================

# odoo-nginx-reverse-proxy
Odoo instance with docker. Odoo customized with workers and a nginx container that acts as a reverse proxy.

Odoo exposes 8069 and 8072 ports (as specified in the odoo.conf and dockerfile files).
Nginx exposes 80 (default) and 8069 ports (as specified in the dockerfile file)

In the docker-compose file, odoo_proxy (nginx) publishs 8069 port.
