

Service Account (MySCM project)

Create SA with Role Cloud SQL Admin, Cloud SQL Editor, Cloud SQL Client

fml-dev-dig-myscm1


Configure GKE (Infracore project)

kubectl create secret generic wordpress-instance-credentials --from-file=credentials.json=[SA_KEY_FILE_PATH]

kubectl create secret generic wordpress-db-credentials --from-literal=username=[DBUSER] --from-literal=password=[PASSWORD]

Create a namespace on Kubernetes

kubectl create namespace my-scm

