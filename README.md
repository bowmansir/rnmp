# rnmp(基于 Docker 便携式开发环境)
nginx+mysql+php+redis

# 先得安装好 docker && docker-compose

# 安装
```
$ git clone git@github.com:bowmansir/rnmp.git
$ cd rnmp
$ docker-compose up -d
```

# 配置说明
>redis 端口对外为: 6380  
php-fpm 对外: 9000  
mysql 对外: 9503  
nginx 对外: 80
>
具体的修改自行通过 docker-composer.yeml

# 目录说明
> app 为项目的根目录  
log 为日志文件  
service 中为 Dockfile 构造文件

# 使用说明
> nginx 实例配置见 service/nginx/conf/default.conf  
var/www => 对应 /app  
var/log/nginx/ => 对应 /log/nginx/ 
