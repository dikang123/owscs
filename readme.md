# Over the wall Small crawler software...

## 描述
该软件的作用是每天登录瓜瓜SS共享站点,登录我的账号并点击签名按钮获取每日流量份额.

如果访问成功,自动收集每日最新站点的信息并将信息通过邮件系统发送到邮箱中,方便需要的时候随时取用.

## 模块分析
为了防止账号信息泄漏,需要通过读取配置文件的方式启动.
### 启动流程
- 读取配置文件获取账号密码和瓜瓜的域名,同时获取发送邮件的邮箱账号与密码
- 目前网站能直接登录不需要翻墙,方便了很多,不过还是要保留扩展使用代理的可能性.
- 登录后直接发送签到请求
- 读取节点信息
- 通过邮件功能发送邮件到收取邮件的邮箱.

## 使用
软件放在家里的linux服务器上自动运行,每日固定时间点运行,读取配置文件中的账号和域名,自动登录.



> 死猪 20180304
