# VPN

kloudlite provide vpn connectivity that will help to make a private connection for your device.

You can see your vpn status using kli command line:

```
# choose cluster
kli use cluster

# Connect your device to the existing cluster
sudo kli vpn start

# Test connection
curl <http-service-name>.<namespace>.svc.cluster.local

# check the vpn status
sudo kli vpn status
```
