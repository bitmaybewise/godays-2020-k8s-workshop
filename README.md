# GoDays 2020 Kubernetes workshop

## PodHealth Controller using kubebuilder

### Create with

```sh
# we'll use a domain of example.com,
# so all API groups will be <group>.example.com.
$ kubebuilder init --domain example.com

# create a new API object for our simple operator
$ kubebuilder create api --group training --version v1alpha1 --kind PodHealth

## after implementing types
make manifests
make generate
```

### To try out

```sh
# Connect to kubernetes cluster

# Install CustomResourceDefnitions
$ make install

# Run Operator locally
$ make run
```
