`ss-panel-v3-mod_Uim 开发团队仅为面板的用户提供 V2Ray 后端对接功能，V2Ray 节点后端与 ss-panel-v3-mod_Uim 面板无关。ss-panel-v3-mod_Uim 开发团队不对节点后端提供任何形式的保证：不保证后端程序能满足您的要求或您的服务不会中断。如果您因为 V2Ray 节点后端的使用而引发的一切纠纷，应自行准备相关材料，及时与 V2Ray 节点后端开发者联系，ss-panel-v3-mod_Uim 开发团队不承担任何相关责任。`

# V2ray Backend 用法
## 站点设定
首先先在 后台创建节点
> 节点的节点地址为 域名;端口;协议;AlterId;Level

事实上在默认情况下 协议为 VMess 端口为 443 AlterId 为 32 Level 为 0

> 这些设置可以在 config.json 中修改

![Snipaste_2018-05-06_15-50-40.png](https://i.loli.net/2018/05/06/5aeeb3df9be7e.png)


> 单端口多用户请选择 只启用普通端口

并将节点类型选为 `V2Ray`

> 联系 order@indexyz.me 获取后端

当你获取了后端之后

## 部署
登陆要部署的服务器 假设这边后端名称为 `bin`

并执行以下命令就可以启动服务器
```bash
chmod +x bin
nano agent.yaml
./bin
```

## Agent 设定
编辑 `agent.yaml` (如果没有就新建一个)
其中的内容为
```yaml
mod:
  nodeId: 节点ID
  key: 通信密钥
```

V2Ray 可用的选项为
```yaml 
v2ray:
  alterId: 用户的 alterId
  tag: 传入协议的 Tag (默认为 proxy)
```
