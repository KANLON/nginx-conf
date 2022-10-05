# 这里记录自己的服务器上的一些nginx配置

## 概述

这里存放自己服务器上的一些nginx配置，用于备份和发布

每个配置文件基本都是一个服务的nginx配置



## 常用的一些配置说明

1. `include` 将其他目录下的配置文件引入主nginx配置生效
```
http {
.....
include /data/services/nginx_host/*.conf;
......
} 
```


2. `nginx -t` 检查nginx配置是否为有效的配置同时可以看到nginx的默认的配置文件路径；`nginx -s reload` 使新增的nginx配置生效