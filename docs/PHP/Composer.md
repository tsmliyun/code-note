# Composer

## 常用命令

### 查看镜像源

```linux
composer config -g -l
```

### 配置镜像源

```linux
# 全局配置
composer config -g repo.packagist composer https://mirrors.aliyun.com/composer/
# 取消全局配置
composer config -g --unset repos.packagist

# 项目内配置
composer config repo.packagist composer https://mirrors.aliyun.com/composer/
# 取消项目配置
composer config --unset repos.packagist

```



