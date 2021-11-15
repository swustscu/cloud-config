# cloud-config
第一种：
  1.服务端只配置uri，客户端配置config.import和cloud.config.lable
  2.服务端配置：spring.cloud.config.server.git.uri: https://github.com/swustscu/cloud-config
  3.客户端配置：spring.config.import: optional:configserver:http://localhost:8888
               spring.cloud.config.label: main
第二种：
  1.服务端只配置uri和default-label,客户端配置config.import
  2.服务端配置：spring.cloud.config.server.git.uri: https://github.com/swustscu/cloud-config
               spring.cloud.config.server.git.default-label: main
  3.客户端配置：spring.config.import: optional:configserver:http://localhost:8888
               
