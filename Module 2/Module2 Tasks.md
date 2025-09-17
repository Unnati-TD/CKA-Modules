Unnati Development and Training Center Pvt Ltd

CKA – Module2 Gradable Task

|**Sr. No.**|**Tasks**|
| :-: | :-: |
|1\.|Create a Secret named `db-credentials` with keys `username=admin` and `password=redhat123`.|
|2\.|Create a ConfigMap named `app-config` with key `APP_MODE=production`.|
|3\.|Create a Pod named `custom-pod` running `nginx` with annotation `purpose=test`.|
|4\.|Create a NodePort Service named `np-service` exposing a pod running `nginx` on port 80.|
|5\.|Taint a node with `key=team`, `value=dev`, `effect=NoSchedule` and create a pod `dev-app` that tolerates it.|
|6\.|Create a PersistentVolume `local-pv` and PersistentVolumeClaim `myclaim` that bind successfully.|
|7\.|Create a pod `host-logger` that mounts `/var/log` from the host using hostPath to `/mnt/logs` in the container.|
|8\.|Create a pod `logger-pod` using `emptyDir` volume mounted at `/tmp/logs`</p>|
|9\.|<p>Create a pod `full-stack-app` running `nginx` with label `app=web`.</p>|


