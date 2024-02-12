This is a Shopware container to install and a plugin

1. git clone git@github.com:ottobusenbach/sw6dockercompose.git
2. git clone git@github.com:ottobusenbach/asam-sw6.git custom/plugins/AsamFieldPlugin
3. docker compose up -d
4. docker exec -it shop bin/console plugin:refresh
5. docker exec -it shop bin/console plugin:install AsamFieldPlugin
6. docker exec -it shop bin/console plugin:activate AsamFieldPlugin
7. docker exec -it shop bin/console cache:clear
