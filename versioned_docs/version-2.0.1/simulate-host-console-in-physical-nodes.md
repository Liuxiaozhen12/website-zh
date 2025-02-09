---
title: 模拟主机故障
sidebar_label: 模拟主机故障
---

本文档介绍如何使用 Chaosd 模拟主机关机故障。

## 查看主机关机实验的帮助信息

在创建故障实验前，可运行以下命令查看主机关机实验的帮助信息：

```bash
chaosd attack host shutdown -h
```

输出如下所示：

```bash
shutdowns system, this action will trigger shutdown of the host machine

Usage:
  chaosd attack host shutdown [flags]

Flags:
  -h, --help   help for shutdown

Global Flags:
      --log-level string   the log level of chaosd, the value can be 'debug', 'info', 'warn' and 'error'
```

## 创建主机关机实验

要创建实验模拟主机关机故障，请执行以下命令：

```bash
chaosd attack host shutdown
```

输出示例如下：

```bash
chaosd attack host shutdown
Shutdown successfully, uid: 4bc9b74a-5fe2-4038-b4f3-09ae95b57694
```

执行该命令后，你的主机会在所有进程关闭后关机。
