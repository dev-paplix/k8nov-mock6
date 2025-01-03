QUESTION 1:

Create a new pod called web-pod with image busy box Allow the pod to be able to set system_time The container should sleep for 3200 seconds


QUESTION 2:
Create a new deployment called myproject, with image nginx:1.16 and 1 replica. Next upgrade the deployment to version 1.17 using rolling update Make sure that the version upgrade is recorded in the resource annotation.

QUESTION 3:
Create a new deployment called my-deployment. Scale the deployment to 3 replicas. Make sure desired number of pod always running.

QUESTION 4:
Create a pod called pod-multi with two containers, as given below:
Container 1 - name: container1, image: nginx
Container2 - name: container2, image: busybox,
command: sleep 4800

QUESTION 5:
Create a YAML file defining a Persistent Volume (PV) named user-data-pv with the following characteristics:
Uses the hostPath storage type with the path /mnt/ssd
Provides ReadWriteOnce access mode
Reclaims the storage automatically when the PV
becomes unbound from a Persistent Volume Claim
(PVC)

QUESTION 6:
Upgrade your Kubeadm to 1.31.1-x version


QUESTION 7:
Make neccessary preparation and Schedule a pod as follows:
✑ Name: nginx-jaud00401
✑ Image: nginx
✑ Node selector: disk=ssd

QUESTION 8:
Create a role access to the namespace of the newrole. Use the current role to create and list the pods

QUESTION 9:

Create a Network Policy named "appychip" in default namespace
There should be two types, ingress and egress.
The ingress should block traffic from an IP range of your choice except some other IP range.
Should also have namespace and pod selector. Ports for ingress policy should be 6379
For Egress, it should allow traffic to an IP range of your choice on 5978 port.


QUESTION 10:

You are managing a Kubernetes cluster for a web application consisting of frontend, backend, and database components.
The frontend pods should be co-located with the backend pods for performance reasons, while the database pods should be spread out
to avoid a single point of failure.

Your Task:

Pod Affinity - Ensure that frontend pods are scheduled on the same nodes as backend pods.
Pod Anti-Affinity - Ensure that database pods are not scheduled on the same node as other database pods.

BACKEND
Backend Deployment: First, let's create the backend deployment which the frontend pods will prefer to be co-located with.

QUESTION 11:
Save the current coredns config map into the /home/coredns.txt




QUESTION 12:
Create a statefulset names postgres with the following charecteristics"

Image: postgres:13.16-bookworm
env: POSTGRES_PASSWORD, POSTGRES_USER, POSTGRES_DB

Expose to outside kubenetes using the exact port of 5432

QUESTION 13:
Create a deployment using the following image:

httpd:bookworm

Expose it to the web on example.org domain

QUESTION 14:

Make a backup from your cluster, and then delete the deployment you created in the last question. Restore the backup and make sure the previous deployment is there

QUESTION 15:

Create a statefulset name MySql with the following configuration:

Image: mysql:8.0.40-debian
MYSQL_ROOT_PASSWORD and MYSQL_PASSWORD from the secret
MYSQL_DATABASE and MYSQL_USER from the configmap

QUESTION 16:


Create a deployment named “apache” in the web namespace that uses the image httpd:2.4.54 and contains three pod replicas Scale the deployment named 'apache' from 3 replicas to 5. Change the image used for the pods in the 'apache' deployment to httpd:alpine .

QUESTION 17:

Create a deployment named redis with the following configuration with a proper persistent volume and persistent volume claim.

namespace: database
image: redis:bookworm
local volume: /var/db
volumeMount: /usr/local/etc/redis

