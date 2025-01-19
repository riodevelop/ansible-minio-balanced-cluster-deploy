# ansible-minio-balanced-cluster-deploy

Simple playbook for deploying MinIO cluster with NGINX load balancing and cluster virtual ip via keepalived.

Writed mainly for RHEL based distros, but could simply edited for another distros.

## Deploying process

1. Fill inventory example with your hosts for minio, interfaces, passwords, etc.
2. Run playbook:
    ansible-playbook -i inventory/yourinventory.ini -kK install.yml

Tested on ansible 2.18.1 and Oracle Linux 9.5