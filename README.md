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

## Docker Tips

See: https://github.com/probcomp/developer#docker-tips
