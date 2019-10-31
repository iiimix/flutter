# 准备工作（这里以windows为例）

- 操作系统：Windows 7 SP1 或更高的版本（64 位操作系统）
- 不少于400 MB
- Git for Windows 2.x（git环境变量已配置）

## 1. 获取Flutter SDK

两种方式

### 1.1 下载安装包（截止2019-10-31最新稳定版）
[flutter_windows_v1.9.1+hotfix.6-stable.zip](https://storage.googleapis.com/flutter_infra/releases/stable/windows/flutter_windows_v1.9.1+hotfix.6-stable.zip)

### 1.2 命令行方式安装
新建一个目录，例如：`D:\platform\flutter`
```
git clone -b stable https://github.com/flutter/flutter.git
```

## 2. 配置flutter环境变量，添加到path  `D:\platform\flutte\bin`
```
D:\platform\flutte\bin
```

### 2.1 打开命令窗口CMD，运行`flutter doctor`检查开发环境

此时可能需要`Running pub upgrade...`

并且会卡死

可能你已经猜到了，国内有Great Wall

### 2.2 使用国内镜像[Using Flutter in China](https://flutter.cn/community/china#configuring-flutter-to-use-a-mirror-site)
新增环境变量
腾讯云开源镜像站
```
PUB_HOSTED_URL=https://mirrors.cloud.tencent.com/dart-pub
FLUTTER_STORAGE_BASE_URL=https://mirrors.cloud.tencent.com/flutter
```
