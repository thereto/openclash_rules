旁路由模式，多订阅

1.直接下载config.yaml修改，一劳永逸
  - 补充订阅url
  - 修改DNS中的nameserver为运营商dns

2.根据订阅节点和实际使用情况，配置规则和策略
  - github的文件，如果路由无法直接访问，可以加上https://gh-proxy.com/
  - 负载均衡对于稳定性不高的节点，不见得好用，建议高质量节点组去配置，负载均衡的详细参数参考所用插件提供的指导文档

3.openwrt网络-DNS设置中关闭DNS重定向（新安装的Openclash，需要在插件设置-版本更新中更新meta内核）

4.openclash初始化，如果不需要认证信息，记得在覆写设置中删除，然后保存配置

5.配置管理，上传前面修改好的config.yaml，然后启动openclash，openclash页面不会显示订阅信息，直接进yacd中查看
