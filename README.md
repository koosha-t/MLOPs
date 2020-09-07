# Deploying Machine Learning Models Using Kubeflow

## Hello Kubeflow

### Setting up KubeFlow on your local

Kubeflow is fairly self-contained but it requires _kubectl_ for communicating with Kubernetes. The rest of the dependencies are inside containers.

* installing kubectl using snap:

```sh
	sudo snap install kubectl --classic
``` 

* installing kubectl using homebrew:

```sh
	brew install kubernetes-cli
```

One you install kubectl, you can install Kubeflow using the script (setup.sh) provided in the installation folder.

run the following after running the setup script to make sure Kubeflow is installed on your machine:

```sh
kfctl version
```



