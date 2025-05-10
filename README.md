## NOTES

### basic php nginx docker with better dependencies



### notes for cli docker
- docker compose up
- docker ps
- docker compose ps 
- docker compose up -d
- docker compose build
- docker compose down

### somehow useful
- reload without dropping packets
```
  nginx -s reload
```
- server static content
```
rewrite this path /etc/nginx/conf.d/default.conf
server {
  listen 80 default_server;
  server_name www.example.com;
  location / {
    root /usr/share/nginx/html;
    # alias /usr/share/nginx/html;
    index index.html index.htm;
  }
}
```
