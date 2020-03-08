# docker-files

## 用法

进入需要的目录下，使用 `docker-compose up`

####  mysql4dev 主从复制模式

用户名为 `devuser`，密码为 `devuser`，主库连接地址: `127.0.0.1:33060`，从库连接地址：`127.0.0.1:33061`  

详细步骤请查看：[基于docker的Mysql主从复制容器搭建
](https://www.jianshu.com/p/b778f8236b10)

--------

#### docker 用户组权限修改

1. Create the `docker` group.

    `$ sudo groupadd docker`

2. Add your user to the `docker` group.

    `$ sudo usermod -aG docker $USER`

    On Linux, you can also run the following command to activate the changes to groups:

    `newgrp docker`

3. Verify that you can run `docker` commands without `sudo`.

    `$ docker run hello-world`
