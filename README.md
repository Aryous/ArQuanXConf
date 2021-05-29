# ArQuanXConf
- Quantumult X 自用配置文件
- 本配置不包含节点信息
- 部分高校和机构购买了数据库，因此增加了 <学术搜索> 分流策略，记得勾选直连。该策略默认启用ACL4SSR的规则，较为全面；神机学术规则由于包含了google scholar，启用时记得开启资源解析器，在其后添加 #out=google
- 注释掉了163.com及126.com的DNS，保证网易云的正常播放。
- 使用移动运营商的注意禁用系统dns，否则可能导致无法更新分流规则。
- 新增了SSID策略组，默认关闭。
- 启用SSID策略组而非running mode trigger的原因：
  - running mode trigger属于全局直连，会导致某些广告分流或屏蔽更新失效
  - SSID策略组对分流控制更加精准，可以满足更多需求
