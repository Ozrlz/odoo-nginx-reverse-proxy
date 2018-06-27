# odoo-nginx-reverse-proxy
Odoo instance with docker. Odoo customized with workers and a nginx container that acts as a reverse proxy.

Odoo exposes 8069 and 8072 ports (as specified in the odoo.conf and dockerfile files).
Nginx exposes 80 (default) and 443 ports (as specified in the dockerfile file)

In the docker-compose file, odoo_proxy (nginx) publishs 80->80 and 443->443 ports.

Do not use it in prod.
