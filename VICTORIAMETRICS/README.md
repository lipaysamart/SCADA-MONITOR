##### Usage:

* `helm repo add vm https://victoriametrics.github.io/helm-charts/` #添加operate包

* `helm fetch vm/victoria-metrics-operator` #下载operate包到当前路径

* `helm upgrade --install victoria-metrics-operator vm/victoria-metrics-operator -f values.yaml -n vm-operator --create-namespace`          #安装operate包
{% note blue %}
VMSingle.yaml -> VMAgent.yaml -> VMAlert.yaml  #依次定义对应CRD
{% endnote %}
