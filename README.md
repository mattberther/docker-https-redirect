# docker-https-redirect
A simple nginx container that redirects http requests to https.

## Usage
This container can be used from the commandline, or using docker-compose.

### CLI
```
docker run \
    --name=redirector \
    -p 32834:80 \
    mattberther/https-redirect
```

### Compose
```
version: '3'

services:
    redirector:
        image: mattberther/https-redirect
        ports:
            - "32834:80"
```

