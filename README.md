RabbitMQ (single container) plugin for Dokku
============================================

Project: https://github.com/progrium/dokku

Requirements
------------
* dokku-link plugin (https://github.com/rlaneve/dokku-link)

Instalation
-----------
```
cd /var/lib/dokku/plugins
git clone https://github.com/jlachowski/dokku-rabbitmq-single-plugin.git rabbitmq
dokku plugins-install
```

Commands
--------
```
$ dokku help    
    rabbitmq:create <app>                         Create a rabbitmq virtual host/user
    rabbitmq:delete <app>                         Delete specified rabbitmq vhost/user
    rabbitmq:rebuild <app>                        Rebuild specified rabbitmq vhost/user
    rabbitmq:start                                Start the rabbitmq docker container if it isn't running
    rabbitmq:stop                                 Stop the rabbitmq docker container
    rabbitmq:status                               Shows status of rabbitmq
    rabbitmq:list                                 List all virtual hosts
```

TODO:
-----
- write the list command
- add peristent logs

Thanks
------
This is partially based on the dokku-postgresql-plugin: https://github.com/jeffutter/dokku-postgresql-plugin
