# Wireguard Connect

Kloudlite provides a unique way to access the services running inside kubernetes. `kli` tool will open a wireguard connection from your local machine and connect it with the cluster.

### Connect using cli

```
# Connect your device to the existing cluster
kli --cluster-name=<cluster-name> vpn connect

# Test connection
curl <http-service-name>.<namespace>.svc.cluster.local
```



