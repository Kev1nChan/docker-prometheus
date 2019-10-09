## Docker-Prometheus
使用Docker-compose部署Grafana+Prometheus
***
使用Grafana+Prometheus+alertmanager+cadvisor+node_exporter组合，对服务器上Docker、宿主机状态等进行监控与报警。

使用前请修改Grafana配置文件中密码，当前`admin`密码为`qwe123!@#`

使用外部配置文件挂载到容器内部

文件结构：
```shell
docker-prometheus/
├── alertmanager
│   └── config.yml
├── docker-compose.yml
├── grafana
│   ├── config.monitoring
│   └── provisioning
└── prometheus
    ├── alert.yml
    └── prometheus.yml
```