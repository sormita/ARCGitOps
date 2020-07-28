compute-resources file is the resource quota for the cluster. The reason it is not in cluster-apps folder, because it has to be applied using --namespace=default.
kubectl apply -f compute-resources.yaml --namespace=default

If namespace is not specified then it will get applied to all the namespaces. 