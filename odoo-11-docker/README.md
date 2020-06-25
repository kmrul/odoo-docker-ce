# Setup Docker for Odoo 11 with pgAdmin Access


### Install docker:
```
$ sudo apt install docker.io
$ sudo systemctl start docker
$ sudo systemctl enable docker
```

### Install docker compose:
```
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.23.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose
$ sudo systemctl enable docker
```

### Start the container from the root of this project:
```
$ docker-compose up  -d
```

Then locate `localhost:11000` to access Odoo 11.0.

<img width="500px" src="https://github.com/kmrul/odoo-docker-ce/blob/master/odoo-11-docker/static/odoo-apps.png" alt="Odoo is working.">

Connect your postgres db now by creating a new server in pgAdmin.
```
name: Odoo11
host: localhost (if not matched, find hostname)
port: 5060
username: odoo
password: odoo
```

<img width="500px" src="https://github.com/kmrul/odoo-docker-ce/blob/master/odoo-11-docker/static/pg-access.png" alt="Postgres is working.">


#####################################################

### [Follow My Blog](http://kamrul.net)
