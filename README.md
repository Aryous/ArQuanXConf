# ArQuanXConf
- Quantumult X 自用配置文件

- 基于STICK RULES、神机规则等项目的配置整理
  改编自[Sabrina的万事屋](https://merlinblog.xyz/)博主规则模板

- 对于购买了部分数据库的高校和机构， <学术搜索> 分流策略组选择直连。
  默认启用ACL4SSR的规则；
  神机学术规则使用时开启资源解析器，在其后添加 #out=google以排除google scholar域名

- 注释掉了163.com及126.com的DNS，保证网易云的正常播放。

- 使用移动运营商时可能需要禁用系统dns，否则有时会导致无法更新分流规则。

- 新增了SSID策略组，默认关闭。

  启用SSID策略组而非running mode trigger的原因：
  - running mode trigger属于全局直连，会导致某些广告分流或屏蔽更新失效
  - SSID策略组对分流控制更加精准，可以满足更多需求
