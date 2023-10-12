# opencart-docker

Proper readme coming soon...

1. Download latest release of open cart 4 from here (url to come)[#]
2. unzip and move contents of the `upload` directory to `opencart/html/` directory
3. Run `chown -R 33:33 opencart` to change the ownership to the apache user in the container
4. Rename the config files:
   - `mv opencart/html/config-dist.php opencart/html/config.php`
   - `mv opencart/html/admin/config-dist.php opencart/html/admin/config.php`
3. Ensure you filled out the `{missing information}` in the `docker-compose.yml`
4. run `docker compose up -d`
5. Reverse proxy or expose the port 80 or something to the running dockerized apache
6. Visit the url you set for the opencart apache container, go through setup and enter the DB information you created in the `docker-compose.yml` file