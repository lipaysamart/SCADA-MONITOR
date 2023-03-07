
spec:
  vmProberSpec:
    url: prometheus-blackbox-exporter.vm-single.svc:9115   #指定blackbox-exporter地址
  module: ping                 #配置文件中的检测模块
  targets:                      #抓取目标配置
  ##### ingress <Object>
   staticConfig:          #如果配置了 ingress，静态配置优先
#### 调试:
curl http://192.168.189.120:9115/probe?target=prometheus.io&module=http_2xx&debug=true