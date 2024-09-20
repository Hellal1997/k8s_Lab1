# k8s_Lab1
## Lab 1 Questions

1. Install Kubernetes Cluster (Minikube).

2. Create a pod with the name `redis` and with the image `redis`.

3. Create a pod with the name `nginx` and with the image `nginx123`. Use a pod-definition YAML file.

4. What is the nginx pod status?

5. Change the nginx pod image to `nginx` and check the status again.

6. How many ReplicaSets exist on the system?

7. Create a ReplicaSet with the following specifications:
   - name: `replica-set-1`
   - image: `busybox`
   - replicas: 3

8. Scale the ReplicaSet `replica-set-1` to 5 pods.

9. How many pods are READY in the `replica-set-1`?

10. Delete any one of the 5 pods, then check how many pods exist now. Why are there still 5 pods, even after you deleted one?

11. How many Deployments and ReplicaSets exist on the system?

12. Create a Deployment with the following specifications:
   - name: `deployment-1`
   - image: `busybox`
   - replicas: 3

13. How many Deployments and ReplicaSets exist on the system now?

14. How many pods are ready with `deployment-1`?

15. Update `deployment-1` image to `nginx`, then check the ready pods again.

16. Run `kubectl describe deployment deployment-1` and check the events. What is the deployment strategy used to upgrade the deployment-1?

17. Rollback the `deployment-1`. What is the used image with the `deployment-1`?

18. Create a deployment using the `nginx` image with the latest tag only, and remember to mention the tag i.e. `nginx:latest`. Name it as `nginx-deployment`. App labels should be `app: nginx-app` and `type: front-end`. The container should be named as `nginx-container`. Also, make sure replica counts are 3.
