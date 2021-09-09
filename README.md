# k3os-ansible

Ansible role to rekick a server into k3os, retaining hostname, static IPs, ssh keys, etc.

```bash
curl -sSL https://raw.githubusercontent.com/rancher/k3os/master/install.sh
```

```bash
╰─> curl -sSL -H "Accept: application/json" https://api.github.com/repos/rancher/k3os/releases|jq '.[]|select(.prerelease == false)|.name'
```

```bash
┬─{ jack:~/s/g/j/bootstrap_k3os git:(main) ✗
╰─> curl -sSL -H "Accept: application/json" https://api.github.com/repos/rancher/k3os/releases|jq '.[]|select(.prerelease == false)|.name'
"v0.19.11-k3s1r0"
"v0.20.7-k3s1r0"
"v0.20.6-k3s1r0"
"v0.19.10-k3s1r0"
"v0.20.4-k3s1r0"
"v0.19.8-k3s1r0"
"v0.11.1"
"v0.11.0"
"v0.10.3"
"v0.10.2"
"v0.10.1"
"v0.10.0"
"v0.9.1"
```