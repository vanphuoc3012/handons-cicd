kubectl create configmap notepad-logback-testing-configmap --from-file=./testing/logback-spring.xml
kubectl create configmap notepad-logback-staging-configmap --from-file=./staging/logback-spring.xml
kubectl create configmap notepad-logback-production-configmap --from-file=./production/logback-spring.xml

kubectl create secret generic github-private-key-secret --from-file=id_rsa


kubectl get pods -o wide
kubectl get node -o wide