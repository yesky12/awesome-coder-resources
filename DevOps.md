

## 发布平台

> ----------walle 2.0 瓦力 | walle 瓦力 - 部署系统
> http://walle-web.io/docs/

walle 让用户代码发布终于可以不只能选择 jenkins

==========




## 【K8s的部署方案-Drone】

> ----------从Jenkins迁移到Jenkins X：一场持续交付之旅：：高效开发运维
> https://mp.weixin.qq.com/s/yq7cBZJiTd_TlafNuX17WA

Jenkins X 是一个高度集成化的 CI/CD 平台，基于 Jenkins 和 Kubernetes 实现，旨在解决微服务体系架构下的云原生应用的持续交付的问题

==========



> ----------如何选择最佳CI工具：Drone VS. Jenkins - RancherLabs的博客 - CSDN博客
> https://blog.csdn.net/rancherlabs/article/details/80300621

多年来，Jenkins一直是行业标准的CI工具。它包含了许多功能，在其生态系统中有近1000个插件，对于那些推崇简单的人来说，这可能令人望而生畏。Jenkins在容器出现之前就已存在，不过它还是很适合容器环境的。但也不得不说，以前Jenkins并没有给予容器什么特殊关注，它并没有很致力于让容器变得更好，不过现在Blue Ocean和pipeline的出现和发展让这一情况有了很大改观。

Drone是一个广受欢迎的开源CI工具。它其实是原生Docker，所有的进程都在容器内进行。这使得Drone非常适合像Kubernetes这样的平台，因为在Kubernetes上启动容器很简单。

Rancher容器管理平台对Drone和Jenkins都能提供优秀的支持，用户通过一个自动化的过程即可方便快速地创建Kubernetes集群。我用Rancher 1.6在GCE上部署了K8s 1.8集群，过程之简单简直令人惊喜。

本文将把Drone部署在Kubernetes（Rancher）上，并将从以下三个方面比较Drone与Jenkins:

1、平台安装和管理
2、插件生态系统
3、Pipeline细节

==========

