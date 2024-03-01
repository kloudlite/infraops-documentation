# Access your first cluster

### Using \`kli\`

Install kli tool to access your clusters

```
# Install kli
curl https://kli.devc.kloudlite.io/v1.0.5-nightly! | bash

# Login
kli auth login

# Choose Cluster
kli use cluster

# Open kli shell
kli shell

# Access cluster
kubectl get nodes
```

### Using kubeconfig file

Download your kubeconfig file provided in the dashboard and start accessing your cluster

```bash
export KUBECONFIG=/path/to/config 
kubectl get nodes
```

<figure><img src="../../.gitbook/assets/Screenshot 2024-02-21 at 11.29.01 AM.png" alt=""><figcaption></figcaption></figure>

