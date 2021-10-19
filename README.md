


semaphore

#  01编译
下载代码
```
git clone https://github.com/ansible-semaphore/semaphore.git
```
编译：
使用task工具：
https://taskfile.dev/#/installation

```
task all
```

在semaphore/bin 目录生成 semaphore 二进制文件


*  出现问题
编译过程中报错，可以把test这个task先干掉

#  02setup

搭建数据库：

```
docker run -d --name=mysql -p 127.0.0.1:3306:3306 -e MYSQL_ROOT_PASSWORD=my-secret-pw mysql:5.6

```



```
./semaphore setup
```


```
You are all setup admin!
 Re-launch this program pointing to the configuration file

./semaphore --config /root/install/compile-semapgore/semaphore/bin/config.json

 To run as daemon:

nohup ./semaphore --config /root/install/compile-semapgore/semaphore/bin/config.json &

 You can login with admin@admin.com or admin.

```



#  使用

登录 IP:3000  ,使用 admin/admin登录系统即可







