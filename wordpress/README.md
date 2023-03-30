# Wordpress Fun

Build is super easy.

```bash
$ sudo docker-compose up
(Get webserver docker IP, and log in / initialize wordpress with admin/admin user-pass in a browser)
$ sudo docker ps (get names: webserver, wordpress, db)
$ sudo docker copy wp-file-manager.zip wordpress:.
$ sudo docker exec -it wordress /bin/sh
    (inside the container)
    # curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar
    # chmod +x wp-cli.phar
    # mv wp-cli.phar /usr/local/bin/wp
    # wp plugin install /wp-file-manager.zip
    # wp plugin activate wp-file-manager
```

Couple of commands but these are the steps to get it ready to rock and roll
