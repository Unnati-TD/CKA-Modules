# CKA-Modules: Grading & Validation Scripts

A collection of grading (validation) and solution scripts for Kubernetes tasks, helping learners of the *Unnati development & training centre pvt.[KUCL 2.3]* course to automate checking their work.  

---

##  Table of Contents

- [Purpose](#purpose)  
- [Repository Structure](#repository-structure)  
- [Quick Start](#quick-start)  
- [How to Use the Grading Scripts](#how-to-use-the-grading-scripts)  
  
## Purpose

The aim of this repo is to provide:

- Pre-defined Kubernetes tasks matching typical CKA exam topics (Pods, Deployments, Services, Labels, Replica Counts, etc.)  
- Grading / validation scripts to verify whether a task has been implemented correctly  
- Solution scripts or YAML manifests to help if you get stuck  

This allows learners to practice, self-evaluate, correct mistakes, and build confidence.

---

## Repository Structure

- Each module folder contains specific tasks and matching grading scripts  
- `tasks/` contains shell scripts that run `kubectl` commands + checks

CKA-Modules/

|-- Module\ 1

|   |-- CKA-Module1\ Tasks.md

|   |-- CKA-Module1\ Tasks.pdf

|   |-- README.md

|   `-- UNNATI-CKA-MODULE1`

|-- Module\ 2
    |-- Module-2.md
    
    |-- Module2\ Tasks.md
    
    |-- Module2\ Tasks.pdf
    
    |-- README.md
    
    `-- UNNATI-CKA-MODULE2`

---
## Quick Start

Follow these steps to get up and running with the CKA Modules grading scripts:

1. **Set up Kubernetes access**
   - Make sure you have a running Kubernetes cluster (local via Minikube/Kind, or cloud-based).
   - Ensure `kubectl` is installed and configured to point to your cluster:
     ```bash
     kubectl get nodes
     ```

2. **Pick a task**
   - Navigate to the `tasks/` directory and choose the task you want to attempt (e.g., `task9`).
   - Each task will describe what resources you need to create (Pods, Deployments, Services, etc.).

3. **Write or apply YAML manifests**
   - You can write your own YAML files to meet the requirements

4. **Apply your manifests**
   ```bash
   kubectl apply -f my-solution.yaml
   ```

## How to Use the Grading Scripts

The grading scripts are simple **Bash scripts** that validate your Kubernetes resources against the task requirements.

### What They Check
Each script runs `kubectl` commands and verifies:
- ✅ Deployment replica counts  
- ✅ Labels on Deployments and Pod templates  
- ✅ Service types (ClusterIP, NodePort, etc.)  
- ✅ Correct container images  
- ✅ Pod readiness and running status  

### Steps to Run
1. **Apply/Create your resources**  
   First, deploy the YAML manifests you wrote:
   ```bash
   kubectl apply -f my-solution.yaml
   ```
2. **Wait for resources to be ready**
Example:
```
kubectl get pods
```

3. **Run the grading script**
From the tasks/ directory:
```
UNNATI-CKA-MODULE1 task1
```

4. **Check the output**

The script prints pass/fail checks with symbols:

- ✔ myapp1-dep has 6 replicas
- ✘ myapp1-dep missing label course=cka
- ✔ myapp2-dep has 5 replicas

# Example Workflow

### Apply your solution
```
kubectl apply -f tasksolution9.yaml
```
### Run validation
```
UNNATI-CKA-MODULE1 task9
```


This way, you know instantly whether your resources meet the task requirements.



