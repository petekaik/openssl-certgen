# openssl-certgen

Alpine linux with openssl to automate self-signed certificate generation

You can clone repository "certs" structure to generate CA and device/server/user certificates - certificate generation scripts are located in subfolders

Scripts iterate through .conf definitions in "config" folder - edit files to suite your needs

You can trigger certificate generation manually from your Docker host with docker exec (e.g. docker exec certgen /opt/certgen/certs/CA/gen_ca) or automate certificate generation for CA/servers/devices/users with ansible (e.g. petekaik/ansible-openssh)
