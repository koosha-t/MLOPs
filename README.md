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

### Setting up Local Kubernetes (Minikube)

We'll use Minikube to set up a local Kubernetes cluster. 

Please visit [here](https://kubernetes.io/docs/tasks/tools/install-minikube/) for the installation guides for Minicube.

When starting minikube make sure to give it plenty of memory and disk space. For example:

```sh
minikube start  --driver virtualbox --cpus 16 --memory 12g --disk-size 15g
```

Note: You don’t need 16 CPU cores to run this, this is just the number of virtual CPUs minikube will use.

