---
id: installation
sidebar_position: 1
title: ⚙ Installation
slug: /
---

# Installation

## 😊  Hi tKeel

tKeel 是一套强壮可复用的物联网开放平台，能帮助您快速构建解决方案。

我们致力于为物联网开发者提供最优解,帮助物联网服务商解决高并发、多租户以及分布式的难题，使得物联网服务商可以专注于业务开发，更好的为客户提供价值。为使用者提供方便快捷地设备接入能力，还有极易理解和操作的数据抽象、丰富且强大的插件、清爽的平台操作页面让数据安全地尽在掌握。

### Why tKeel?

简单的说，我们有这些可能让你心动的理由：

 * 高扩展、可拔插的基础框架，默认支持多租户能力。
 * 简单快速的二次开发能力，不限定开发语言和架构。
 * 数据实体来描述设备、网关、空间等物理空间对象。
 * 对于数据实体可以随时获取当前数据快照并且订阅数据变化。
 * 简单快捷地推送数据实体到其他系统、平台。

## Install And Initialize Your tKeel

> 我们希望我们提供的安装方式能符合我们平台——气质，简单、便捷。

在您的环境运行 tKeel 平台有多种选择，您可以选择任意一个让您感到舒适的方式安装。

### Get Started by tKeel CLI
使用 _tKeel_ CLI 是我们最推荐的方式，因为它将使您的安装简单到只需一条命令。不过请先正确 [安装 tKeel CLI](cli#install-cli)

但是使用 tKeel CLI 之前请先确保在您的环境中满足如下要求：
#### Prerequisites
- ✅ 如果您需要在 Kubernetes 中安装 tKeel ，确保您的环境中已 [安装 dapr](https://docs.dapr.io/operations/hosting/kubernetes/kubernetes-deploy) 且 dapr 版本必须 `>= 1.4`。
- ✅ 环境中已安装 dapr，且开启 mTLS

> 备注：
> * dapr 在 Kubernetes 上安装时，默认开启了 mTLS。


#### Initialize tKeel Platform by CLI
使用上面安装的命令行工具初始 tKeel 平台。
```bash
tkeel init --debug --wait --timeout 600
```

> 注意：Linux 用户请注意，如果您的 docker 需要使用 sudo 权限才能使用，那么请您使用:
>  ```bash 
> sudo tkeel init
> ```

命令行会输出如下内容：
```bash
⌛  Making the jump to hyperspace...
ℹ️  Checking the Dapr runtime status...
ℹ️  Deploying the tKeel Platform to your cluster... 
ℹ️  install plugins...                                                        
ℹ️  install plugins done.                                                                                 
✅  Deploying the tKeel Platform to your cluster...                          
✅  Success! tKeel Platform has been installed to namespace keel-system. To verify, run `tkeel plugin list -k' in your terminal. To get started, go here: https://tkeel.io/keel-getting-started
```

恭喜您，安装完成了，敬请享用。


### Get Started With Kubernetes




