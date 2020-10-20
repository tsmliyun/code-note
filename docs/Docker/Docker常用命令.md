# Docker常用命令

## 列出所有在运行的容器信息

```linux
# 列出所有在运行的容器信息
docker ps  

# 列出最近创建的5个容器信息
docker ps -n 5

# 列出所有创建的容器ID。
docker ps -a -q
```

![image-20201020132254478](/Users/yunli/Library/Application Support/typora-user-images/image-20201020132254478.png)

字段介绍：

> CONTAINER ID:容器ID
>
> IMAGE:使用的镜像
>
> COMMAND:启动容器时运行的命令
>
> CREATED: 容器的创建时间
>
> STATUS:容器状态，状态有7种：
>
> - created（已创建）
> - restarting（重启中）
> - running（运行中）
> - removing（迁移中）
> - paused（暂停）
> - exited（停止）
> - dead（死亡）
>
> PORTS:容器的端口信息和使用的连接类型（tcp\udp）
>
> NAMES:自动分配的容器名称

OPTIONS说明：

> -a:显示所有的容器，包括未运行的
>
> -f:根据条件过滤显示的内容
>
> --format:指定返回值的模板文件
>
> -l : 显示最近创建的容器
>
> -n: 列出最近创建的n个容器
>
> --no-trunc ：不截断输出
>
> -q:静默模式，只显示容器编号
>
> -s: 显示总文件大小

## 进入容器

```linux
docker exec -it nginx-master /bin/bash
```

