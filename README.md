# Overview

## Initial Setup

### trust the cert
```
sudo security add-trusted-cert -d -r trustRoot \
        -k /Library/Keychains/System.keychain certs/probcomp.rootCA.pem
```

### start the app
```
docker-compose up
```

Services are accessible at `https://<SERVICE>.probcomp.dev:8443`
