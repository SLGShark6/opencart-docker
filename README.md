# opencart-docker

Proper readme coming soon...

1. Download latest release of open cart 4 from here (url to come)[#]
2. unzip and move contents of the `upload` directory to `opencart/www/` directory
3. Ensure you filled out the `{missing information}` in the `docker-compose.yml`
4. run `docker compose up -d`
5. Reverse proxy or expose the port 80 or something to the running dockerized apache
6. Visit the url you set for the opencart apache container, go through setup and enter the DB information you created in the `docker-compose.yml` file