

### Go to Cloudflare and create the name you want to use 
### and the local address of your NGINX Proxy server.
#### You will need your token from cloudflare to use in NGNIX Proxy later.
# Use Portainer stacks to build vaultwarden


>     version: "2.1"
>     services:
>         vaultwarden:
>            image: vaultwarden/server:latest
>            container_name: vaultwarden
>            volumes:
>            - ./vw-data/:/data/
>            ports:
>            - 8088:80
>            - 3012:3012
>            restart: unless-stopped

use NGINX Proxy to setup reverse local proxy
#### local ip of vaultwarden server and port 8080
#### You will also setup ssl and need the token from Cloudflare to complete.




