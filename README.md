


## Quick instructions to just get this working on an OpenShift 3 deployment as a normal user

````
$ oc login https://yourOpenShiftServer
$ oc new-project mlbparks
$ oc create -f https://raw.githubusercontent.com/gshipley/openshift3mlbparks/master/mlbparks-template-eap.json
$ oc new-app mlbparks
````

## Install template as cluster-admin for everyone to use

Load the template with cluster-admin user:

````
# oc create -f https://raw.githubusercontent.com/gshipley/openshift3mlbparks/master/mlbparks-template.json -n openshift
````

