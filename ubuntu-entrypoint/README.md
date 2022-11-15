1. Build the image: `docker build -t guimassoqueto/ubuntu-sleeper:1.0.0 dockerfile/.`
2. Login at dockerhub: `docker login`
3. Push the image: `docker push guimassoqueto/ubuntu-sleeper:1.0.0`
4. See the pod-definition.yaml file inside the k8s/ folder refering to the image pushed
5. Create the pod (using minikube): `minikube start` and `kubectl create -f k8s/pod-definition.yaml` 