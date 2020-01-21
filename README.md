# GoDays 2020 Kubernetes workshop

    # we'll use a domain of loodse.io,
    # so all API groups will be <group>.example.com.
    $ kubebuilder init --domain example.com

    # create a new API object for our simple operator
    $ kubebuilder create api --group training --version v1alpha1 --kind PodHealth

    # Install CustomResourceDefnitions
    $ make install

    # Run Operator locally
    $ make run
