# Overview

## Initial Setup

### trust the cert
```
sudo security add-trusted-cert -d -r trustRoot \
        -k /Library/Keychains/System.keychain certs/probcomp.rootCA.pem
```

### start the app (in the background)
```
docker-compose up -d
```

Services are accessible at `https://<SERVICE>.probcomp.dev:8443`

## Increasing Docker resources

It's recommended that you allocate at least 8GB of RAM and all CPU cores to Docker. Any unused resources will still be available to OSX.

![resources](https://github.com/probcomp/nginx-proxy/raw/master/images/resources.png)
