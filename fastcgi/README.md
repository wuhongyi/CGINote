<!-- README.md --- 
;; 
;; Description: 
;; Author: Hongyi Wu(吴鸿毅)
;; Email: wuhongyi@qq.com 
;; Created: 四 5月  3 22:43:43 2018 (+0800)
;; Last-Updated: 三 5月 30 10:10:49 2018 (+0800)
;;           By: Hongyi Wu(吴鸿毅)
;;     Update #: 10
;; URL: http://wuhongyi.cn -->

# FastCGI

> https://www.nginx.com/resources/wiki/start/topics/examples/fastcgiexample/
> https://caddyserver.com/docs/fastcgi
> https://my.oschina.net/davehe/blog/108107

> https://blog.csdn.net/zhongjling/article/details/52334664
> https://blog.csdn.net/chinalinuxzend/article/details/1811552

----

> http://www.lighttpd.net/

```
默认配置文件路径  /etc/lighttpd
```

我的默认配置

```bash
##  Basic Configuration
## ---------------------
##
server.port = 82


##
## Use IPv6?
##
# server.use-ipv6 = "enable"


## With SELinux enabled, this is denied by default and needs to be allowed
## by running the following once : setsebool -P httpd_setrlimit on  
server.max-fds = 2048
```


```bash
lighttpd -f /etc/lighttpd/lighttpd.conf
```

浏览器中输入

```
http://localhost/
```


<!-- README.md ends here -->
