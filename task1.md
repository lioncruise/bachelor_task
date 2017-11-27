# 实习生作业一

## 任务

1. 调研Kubernetes生态圈的基础组件，并回答以下问题：

* apiserver的主要功能？它是如何与其他组件进行交互的？
* controller manager和replica(yaml文件中的配置项)之间的关系？
* scheduler的作用？及其运作的原理？
* 查看kubelet的启动参数并尝试理解其含义。
* 查看proxy的启动参数并解释proxy的作用（和node、pod之间的关系）。
* 什么是ETCD？它的作用？描述其存储模型。


2. 调研Kubernetes资源，并回答以下问题：

* 什么是node？如何添加删除node？如何修改node的标签？
* 什么是pod？谈谈你对pod的理解。
* 什么是namespace？思考设置namespace的意义。
* 什么label和selector？它们的作用和意义是什么？
* 什么是deployment、replication controller、replication set？它们的共同点及区别？
* 什么是service？service的作用？service是如何关联上pod的？service是通过什么实现的？


3. 使用kubectl、调用REST API、SDK（比如io.fabric8）等方式操作Kubernetes资源，实现以下效果：

* 创建包含一个2个tomcat的deployment。
* 创建关联的service（需要配置node port），使其能够被外部访问。
* 在tomcat的pod上使用环境变量、端口、卷、健康检查、启动参数。
* 调研event对象和watch操作，观察上述创建过程中收到的event以及pod状态的变化。