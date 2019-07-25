# Nginx Reverse-Proxy Container
Accepts incoming traffic on port 80 and serves to port 3000

## Docker

### Build
```
docker build -t nginx .
```

### Run
```
docker run --name=webserver --network=leftovers-network --env-file .env -d -p 80:80 nginx
```