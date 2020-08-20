# flink-notebook
flink从头开始学习总结与笔记,代码

# 环境
* java8
* windows10
* flink-1.11.0-scala-2.12

# 项目结构
* 此文件为介绍和总目录文件
* 项目中每个目录为分类,介绍flink的各种使用方式,并且都为一个key单独运行的项目
* 每个目录下均为一个单独的项目,包括:
    * 学习笔记md文件
    * 练习代码,可能包括:
        * java代码
        * scala代码
        * flink SQL代码

# 从这里开始

## flink 本地安装
### 前言
如果只是为了**练习写flink应用**,可以不用安装flink,直接写flink程序,本地边调试边运行,和写一个java web项目一样即可.

### 环境准备
* java8 或 java11
* linux系统(或WSL,mac)
* flink 安装包

检查java环境
```
java -version
```
> 如果是win10 系统,系统版本>1903,建议安装WSL,安装步骤: https://docs.microsoft.com/zh-cn/windows/wsl/install-win10

下载flink安装包: https://flink.apache.org/downloads.html (非 Source Release 即可)
### 安装启动
比如下载的flink是1.11.0版本,解压
```
tar -xzf flink-1.11.0-bin-scala_2.11.tgz
$ cd flink-1.11.0-bin-scala_2.11
```
启动
```
./bin/start-cluster.sh
Starting cluster.
Starting standalonesession daemon on host.
Starting taskexecutor daemon on host.
```
### 参考
官方文档: https://ci.apache.org/projects/flink/flink-docs-release-1.11/try-flink/local_installation.html