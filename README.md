# Kubernetes

Kubernetes (K8s) is an open-source system for automating deployment, scaling, and management of containerized applications(orchestration).  
### Install Kubernetes:  

The fastest way to install K8s is using the the software *__minikube__*  
minikube can be installed on Windows, Linux or MacOS.  

#### Installing minikube on Windows:  

1. Install and setup *__kubectl__*  

- Download using curl installed, use this command:
<pre>curl -LO https://storage.googleapis.com/kubernetes-release/release/v1.18.0/bin/windows/amd64/kubectl.exe</pre>
- Add the binary in to your PATH
- Test to ensure the version of kubectl is the same as downloaded: __kubectl version --client__  

2. If you do not already have a hypervisor installed, Install a Hypervisor:   
 
- Hyper-V  
- VirtualBox  

3. To install Minikube manually on Windows using Windows Installer, download __https://github.com/kubernetes/minikube/releases/latest/download/minikube-installer.exe__ and execute the installer.  

4. Confirm Installation  

- To confirm successful installation of both a hypervisor and Minikube, you can run the following command to start up a local Kubernetes cluster:  
<pre>
minikube start --driver=driver_name  
#enter the name of the hypervisor you installed in lowercase letters where driver_name  
</pre>

- Once minikube start finishes, run the command below to check the status of the cluster:  
<pre>minikube status</pre>

- If your cluster is running, the output from minikube status should be similar to:  

<pre>
host: Running  
kubelet: Running  
apiserver: Running  
kubeconfig: Configured  
</pre>

### Kubernetes Architecture:  
<img src="imgs/K8s-architecture.jpg" alt="K8s Architecture" width=600 height=350>
