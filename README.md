# CKA-Modules: Grading & Validation Scripts

A collection of grading (validation) and solution scripts for Kubernetes tasks, helping learners of the *Unnati development & training centre pvt.[KUCL 2.3]* course to automate checking their work.  

---

##  Table of Contents

- [Purpose](#purpose)  
- [Repository Structure](#repository-structure)  
- [Quick Start](#quick-start)  
- [How to Use the Grading Scripts](#how-to-use-the-grading-scripts)  
- [Solution Scripts](#solution-scripts)  
  
## Purpose

The aim of this repo is to provide:

- Pre-defined Kubernetes tasks matching typical CKA exam topics (Pods, Deployments, Services, Labels, Replica Counts, etc.)  
- Grading / validation scripts to verify whether a task has been implemented correctly  
- Solution scripts or YAML manifests to help if you get stuck  

This allows learners to practice, self-evaluate, correct mistakes, and build confidence.

---

## Repository Structure




- Each module folder contains specific tasks and matching grading scripts  
- `solutions/` contains example or reference implementations  
- `tasks/` contains shell scripts that run `kubectl` commands + checks  

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



