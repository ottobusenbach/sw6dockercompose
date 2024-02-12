This is a Shopware container to install and a plugin

1. git clone git@github.com:ottobusenbach/sw6dockercompose.git
2. cd sw6dockercompose
3. git clone git@github.com:ottobusenbach/asam-s6.git custom/plugins/AsamFieldPlugin
4. docker compose up -d
5. docker exec -it shop bin/console plugin:refresh
6. docker exec -it shop bin/console plugin:install AsamFieldPlugin
7. docker exec -it shop bin/console plugin:activate AsamFieldPlugin
8. docker exec -it shop bin/console cache:clear
