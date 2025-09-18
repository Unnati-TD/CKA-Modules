**Unnati Development and Training Center Pvt Ltd**


**CKA – Module1 Gradable Task**


|**Sr. No.**|**Tasks**|
| :-: | :-: |
|1\.|Create two pods with names 'testpod1' and 'testpod2'. Both pods should have label "class=unnati". Create these pods using a yaml file and use 'docker.io/httpd' image.|
|2\.|Create five pods with names mypod1, mypod2, mypod3, mypod4, and mypod5. All pods should have label "course=cka". Create these pods using a yaml file and use 'docker.io/openshift/hello-openshift' image.|
|3\.|Create a pod named "nginx-pod" using yaml file and attach a service named "nginxservice" use yaml file to create service. Use port number 18080 for the service. Use label "app=nginx". Use 'docker.io/nginx' image for deploying "nginx-pod" pod.|
|4\.|Create a pod named "banner-pod" using yaml file and attach a service named "banner-service" use yaml file to create service. Use port number 28080 for the service. Use label "banner=podman". Use 'quay.io/libpod/banner' image for deploying "banner-pod" pod.|
|5\.|Create a deployment named "nginx-dep" using "docker.io/nginx" image. Expose the "nginx-dep" deployment to create a service named "nginx-svc". The "nginx-svc" should be of NodePort type.|
|6\.|Create a deployment named "banner-dep" using "quay.io/libpod/banner" image. Expose the "banner-dep" deployment to create a service named "banner-svc". The "banner-svc" should be of NodePort type.|
|7\.|Create a deployment named "supermario-dep" using "docker.io/pengbai/docker-supermario" image. Expose the "supermario-dep" deployment to create a service named "supermario-svc". The "supermario-svc" should be of NodePort type.|
|8\.|<p>Deploy a multitier redis-guestbook application using following link.</p><p>Link:<https://github.com/IBM/guestbook></p><p>Clone this repository using command "git clone https://github.com/IBM/guestbook" . And deploy the guestbook Version 2 multitier application.</p>|
|9\.|<p>Create a deployment named 'myapp1-dep' with label 'class=unnati' and 'course=cka' with 6 replicas. Use 'quay.io/libpod/banner' image for 'myapp1-dep' deployment. Create a service named 'myapp1-svc' and attach to deployment 'myapp1-dep'. </p><p>Create a deployment named 'myapp2-dep' with label class=myclass and course=kucl2.0 with 5 replicas. Use 'docker.io/openshift/hello-openshift' image for 'myapp2-dep'. Create a service named 'myapp2-svc' and attach to deployment 'myapp2-svc'.</p><p>`	`a) List all the pods which has label class=unnati and save output in /root/file1.txt</p><p>`	`b) List all the pods with lables class=unnati and course=cka and save output in /root/file2.txt</p><p>`	`c) List all the pods with lables class=unnati or class=myclass and save output in /root/file3.txt</p>|

