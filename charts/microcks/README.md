# Microcks-Helm

This chart bootstraps a new [Microcks](http://microcks.io) application using the [Helm](https://helm.sh) package manager.

Resources within this directory should work with Helm version 3+.

## Installing the Chart


```console
$ git clone https://github.com/57800-hydroquebec/platform-components.git

$ cd platform-components

$ oc new-project microcks

$ helm install microcks ./microcks-helm --namespace microcks --set microcks.url=microcks.$(ocp dns) --set keycloak.url=keycloak.$(ocp dns)
```

3 default users are available in the microcks instance.


user with password microcks123,


manager with password microcks123,


admin with password microcks123
