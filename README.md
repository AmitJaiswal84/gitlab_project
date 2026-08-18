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
