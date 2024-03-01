# Wireguard Connect

Kloudlite provides a unique way to access the services running inside kubernetes. `kli` tool will open a wireguard connection from your local machine and connect it with the cluster.

## Installations

### Installation on Linux/MacOS

You can install Kloudlite CLI (`kli`) on Linux and MacOS using either `curl` or `wget`. Follow the instructions below based on your preference.

*   #### Using CURL

    Open your terminal and execute the following command:

```
curl 'https://kl.kloudlite.io/kloudlite@v1.0.4-nightly?select=kli' | bash
```

*   #### Using Wget

    If you prefer `wget`, use this command instead:

```
wget -qO- 'https://kl.kloudlite.io/kloudlite@v1.0.4-nightly?select=kli' | bash
```

*   #### Install Specific version&#x20;

    To install a specific version of \[Your Tool Name], use the following command, replacing `v1.0.0` with the desired version number:

```
curl 'https://kl.kloudlite.io/kloudlite@v1.0.4-nightly?select=kli' | bash
```

### Installations on Windows

For Windows users, the installation process involves using PowerShell. Follow the steps below:

#### Install using PowerShell

```
iwr 'https://kl.kloudlite.io/kloudlite@v1.0.4-nightly?select=kli | iex
```

### Post-Installation Steps

After successfully installing `kli`, you can start choosing your cluster and start vpn connection.

### Connect using cli

```
# choose account
kli use account

# choose cluster
kli use cluster

# Connect your device to the existing cluster
sudo kli vpn start

# Test connection
curl <http-service-name>.<namespace>.svc.cluster.local

# Disconnect from the vpn
sudo kli vpn stop
```



