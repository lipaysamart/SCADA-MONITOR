Usage:

####添加operate包####

helm repo add vm https://victoriametrics.github.io/helm-charts/

####下载operate包到当前路径####

helm fetch vm/victoria-metrics-operator

####安装operate包####

helm upgrade --install victoria-metrics-operator vm/victoria-metrics-operator -f values.yaml -n vm-operator --create-namespace

####依次定义对应CRD####

VMCluster.yaml -> VMAgent.yaml -> VMAlert.yaml
