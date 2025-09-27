minikube_namespace_task

🟣 Minikube/Kubernetes Task – Exploring Namespace Creation

This repository documents my GUVI DevOps module assignment focused on hands-on exploration of **Kubernetes namespaces** within a Minikube cluster. All steps were completed using the WSL Ubuntu terminal, with commands and results verified via screenshots. The workflow covers namespace creation, usage, pod deployment, cleanup, and cluster verification, demonstrating practical DevOps processes.

---

✅ Tasks Performed

1. Started Minikube and configured `kubectl` to point to the running cluster:
minikube start
kubectl get nodes

text

2. Listed all available namespaces:
kubectl get namespaces

text

3. Created a new custom namespace:
kubectl create namespace kausheek-lab

text

4. Deployed a pod in the custom namespace:
kubectl run mongo-db --image=mongo:latest --restart=Never -n kausheek-lab

text

5. Verified pod status in all namespaces:
kubectl get pods --all-namespaces
kubectl get pods -n kausheek-lab

text

6. Deleted the namespace and confirmed resource cleanup:
kubectl delete namespace kausheek-lab
kubectl get pods -n kausheek-lab
kubectl get namespaces

text

7. Used ASCII art (`figlet`) for status banners throughout the process for clear visibility.

---

🖥️ Tech Stack

- WSL Ubuntu (Windows Subsystem for Linux)
- Minikube (Kubernetes local cluster)
- kubectl (Kubernetes CLI)
- Docker Desktop (container status)
- Git & GitHub

---

📷 Screenshots

All major steps and outputs, including namespace creation, pod deployment, status verification, and deletion, are documented with attached screenshots.

---

📖 References

- GUVI DevOps Program: [Advanced DevOps & Cloud Engineering Program (Zen Class)](https://www.guvi.in/zen-class/devops-course/)  
- Minikube Docs: [Official Minikube Start Documentation](https://minikube.sigs.k8s.io/docs/start/)  
- Kubernetes Namespace Concepts: [Official Kubernetes Namespaces Guide](https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces/)  
- Kubectl Namespace Reference: [kubectl create namespace](https://kubernetes.io/docs/reference/kubectl/generated/kubectl_create/kubectl_create_namespace/)  
- KodeKloud Blog: [How to Create a Custom Namespace](https://kodekloud.com/blog/kubectl-create-namespace/)

---

📩 Submission

Submitted for the GUVI DevOps Minikube namespace management assignment. All required files and screenshots have been pushed to GitHub as per submission guidelines
