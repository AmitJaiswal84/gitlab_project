===========GitLab Variables=============

Create these under Settings → CI/CD → Variables:

SERVER_HOST
SERVER_USER
SSH_PRIVATE_KEY

For example:

SERVER_HOST = 192.168.1.50
SERVER_USER = root
SSH_PRIVATE_KEY = <private SSH key>

=================Prepare your server=============

Before the first GitLab deployment, run this once on the server:

mkdir -p /opt/nodejs-app


===================Copy your Compose and Nginx files to the server:===================

/opt/nodejs-app/
├── docker-compose.yml
└── nginx.conf

You can do this manually initially.

The GitLab pipeline will then copy:

nodejs-app.tar.gz

to:

/opt/nodejs-app/
