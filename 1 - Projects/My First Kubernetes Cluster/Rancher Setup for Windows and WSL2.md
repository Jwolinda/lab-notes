## Windows Setup

https://rancherdesktop.io/
https://github.com/rancher-sandbox/rancher-desktop/releases
https://docs.rancherdesktop.io/getting-started/installation

Download and install with WSL2 enabled and configure it  to run with WSL2.

Preferences > WSL > Ubuntu + Restart

## WSL Setup

### setup .bashrc

```
alias k='kubectl'

source /etc/bash_completion # not needed on macos

source <(kubectl completion bash)

complete -o default -F __start_kubectl k
```

### User Privileges

Check if you have the right privileges:

```
[ -r /dev/kvm ] && [ -w /dev/kvm ] || echo 'insufficient privileges'
```

Grant user permissions if not:

~~~
sudo usermod -a -G kvm "$USER"
~~~

### Pass

By default, Rancher Desktop uses pass to securely store credentials. If needed, set up on system:

```
gpg --generate-key
```

~~~
apt install pass
pass init <key>
~~~


### Traefik Port Binding Access

By default, most linux systems won't have users allowed to listen on the TCP and UDP ports below 1024. Allow via this command:

~~~
sudo sysctl -w net.ipv4.ip_unprivileged_port_start=80
~~~

### Proxies List

If operating in secure network, the following will need to be allowed:

| Reason | URL |
| -------- | ----- |
| Get available K3s releases for download | [https://api.github.com/repos/k3s-io/k3s/releases](https://api.github.com/repos/k3s-io/k3s/releases)
| Download K3s releases | [https://github.com/k3s-io/k3s/releases/download](https://github.com/k3s-io/k3s/releases/download)
| `kubectl` releases downloaded by `kuberlr` | [https://storage.googleapis.com/kubernetes-release/release](https://storage.googleapis.com/kubernetes-release/release)
| Check available upgrade versions | [https://desktop.version.rancher.io/v1/checkupgrade](https://desktop.version.rancher.io/v1/checkupgrade)
| Access the documentation from the application help menu and help buttons; also used to check online status | [https://docs.rancherdesktop.io](https://docs.rancherdesktop.io)

## Important Note

* Make sure your ~/.kube/config file is not already configured for docker.

Links:

[[Kubernetes]]
[[Rancher]]

202501191259