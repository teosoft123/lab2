<img src="../assets/k8sland.png" align="right" width="128" height="auto"/>

<br/>

# <img src="../assets/lab.png" width="32" height="auto"/> RBAC Lab

> Proxy Music Rocks! Define RBAC rules and binding for the ApiProxy service.
> An ApiProxy provide for listing pod names in a given namespace by contacting
> K8s APIServer.

1. Deploy the given ApiProxy manifest (proxy.yml)
2. Hit the service url for a given namespace
3. What's happening?
4. Now update the provided manifest (rbac.yml) and add Role, Binding and
   ServiceAccount definitions for the ApiProxy service.
   1. Hint ApiProxy needs to list pod names in any given namespace!
5. Hit the service for a few namespaces and make sure it is working nominally
6. Delete your application and RBAC rules!

---
## Commands

### Check The Service

    ```shell
    http $(minikube ip):30404/v1/pods namespace==kube-system
    ```

<br/>

---
<img src="../assets/imhotep_logo.png" width="32" height="auto"/> © 2018 Imhotep Software LLC.
All materials licensed under [Apache v2.0](http://www.apache.org/licenses/LICENSE-2.0)