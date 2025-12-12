task init
# edit cluster.yaml and nodes.yaml 
# export .env
task configure
task bootstrap:talos
task bootstrap:apps
kubectl get pods --all-namespaces --watch
cilium status

