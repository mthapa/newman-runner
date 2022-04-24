## Intro

Simple node app to run postman collections using newman library.
Creates a deployment In Kubernetes Cluster

## References

* https://philna.sh/blog/2019/01/10/how-to-start-a-node-js-project/
* https://www.magalix.com/blog/nodejs-app-sample-from-docker-to-kubernetes-cluster
* https://www.npmjs.com/package/newman#using-newman-as-a-library


## Commands

docker build -t newman-runner .

docker run -d --name newman newman-runner

**Inspect logs**

docker logs -t  newman

docker login 

docker tag newman-runner madanthapa/newman-runner:1.0

docker push madanthapa/newman-runner:1.0

minikube start

kubectl create -f deploy.yaml

kubectl get pods

kubectl logs newman-runner-deployment-5f7999464b-hn578



