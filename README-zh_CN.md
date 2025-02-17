# 阿里云Kubernetes CSI插件


[English](./README.md) | 简体中文

## 插件介绍

阿里云CSI插件实现了Kubernetes平台使用阿里云云存储卷的生命周期管理，支持动态创建、挂载、使用云数据卷。 当前的CSI实现基于K8S 1.10以上的版本；

支持的阿里云存储：***云盘、NAS、OSS、LVM***


### 云盘CSI插件

云盘CSI插件支持动态创建云盘数据卷、挂载数据卷。云盘是一种块存储类型，只能同时被一个负载使用(ReadWriteOnce)。

云盘CSI插件更多详细说明请参考[云盘](./docs/disk.md)


### NAS CSI插件

NAS CSI插件支持为应用负载挂载阿里云NAS存储卷，目前不支持动态创建NAS卷。NAS存储是一种共享存储，可以同时被多个应用负载使用(ReadWriteMany)。

NAS CSI插件更多详细说明请参考[NAS](./docs/nas.md)


### OSS CSI插件

OSS CSI插件支持为应用负载挂载阿里云OSS Bucket，目前不支持动态创建OSS Bucket。OSS存储是一种共享存储，可以同时被多个应用负载使用(ReadWriteMany)。

OSS CSI插件更多详细说明请参考[OSS](./docs/oss.md)

### LVM CSI插件

LVM CSI插件支持创建LVM卷，并挂载。LVM不是高可用存储类型，使用时应用需要注意是否容忍。

LVM CSI插件更多详细说明请参考[LVM](./docs/lvm.md)


## 社区, 贡献, 讨论, 支持

可以到 [Kubernetes](https://kubernetes.io/community/) 社区学到如何获取支持；

可以到 [Cloud Provider SIG](https://github.com/kubernetes/community/tree/master/sig-cloud-provider) 联系到项目管理者；


### 行为准则

参与Kubernetes社区参考[Kubernetes行为准则](code-of-conduct.md)；

可以向社区提交 [Issue](https://github.com/kubernetes-sigs/alibaba-cloud-csi-driver/issues)；
