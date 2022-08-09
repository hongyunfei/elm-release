# elm-release
 饿了么吃货豆工具
 
 ![GitHub watchers](https://img.shields.io/github/watchers/zelang/elm-release)
 ![GitHub forks](https://img.shields.io/github/forks/zelang/elm-release)
 ![GitHub Repo stars](https://img.shields.io/github/stars/zelang/elm-release)
 ![GitHub release (latest by date)](https://img.shields.io/github/downloads/zelang/elm-release/latest/total)

![elm.png](https://raw.githubusercontent.com/zelang/elm-release/main/elm.png)

# 使用说明

1. 请在 [Releases](https://github.com/zelang/elm-release/releases) 根据你的设备下载二进制文件
2. 解压文件
3. 修改`config.yaml`配置文件(注意格式 - auth: 后面有个空格)
4. 饿了么cookie获取(推荐抓包饿了么APP)：[https://air.tb.ele.me/app/conch-page/svip-home-tasklist-new/home](https://air.tb.ele.me/app/conch-page/svip-home-tasklist-new/home)
5. 可选参数 
   - `-debug` 将日志输出到本目录下的文件，方便调试 
   - `-task` 手动执行任务 (默认执行定时任务，需要将程序挂在后台)
   - `-c` 指定配置文件路径
   
# 问题反馈

[https://t.me/elm_tool](https://t.me/elm_tool)

# 目前已实现功能

1. 支持多个cookie执行任务
2. 支持自动更新cookie(需要有登录状态下的cookie)
3. 支持手动/定时执行任务
4. 支持每日签到、自动获取任务列表、自动获取远程隐藏任务列表
5. 支持TgBot / ServerChan消息通知
6. 支持吃货豆兑换10元无门槛红包
7. 配置文件支持热更新 定时执行任务时修改配置后无需重启程序
8. 目前每天可获取吃货豆100-200+

# 更新记录

1.1 
- 修复执行任务提示 - 慢了一步，该红包已被抢光
- 修复debug模式下时区问题

1.2
- 支持手动填写监控任务时间
- 支持吃货豆兑换10元无门槛红包
- `-c` 参数指定配置文件路径
- 配置文件新增参数
  - exchange 是否开启饿了么10元优惠券兑换
  - cron 定时任务 参考：https://tool.lu/crontab/

1.3
- 支持TgBot / ServerChan消息通知
- 修复获取任务列表失败
- 更新`config.yaml`配置文件参数

# 注意事项

1. 本程序需要挂本地执行，如Windows(`*-windows-amd64.zip`)直接本地执行，或者挂N1盒子 选择 `*-linux-arm64.tar.gz`
2. 提示执行失败且失败后面没有提示原因，这个是因为cookie不完整，需要重新抓包，用浏览器抓使用说明中的网址的cookie即可
3. 不提供技术支持，仅接收bug反馈，可以在[群里](https://t.me/elm_tool)或者[issues](https://github.com/zelang/elm-release/issues)中发图+文字说明
4. 本程序不支持在青龙中运行，推荐每天运行两次即可 兑换无门槛红包的先看有没有兑换资格再开启
5. `1.3`版本为稳定版本，功能上不会再进行更新，后续版本以bug修复为主

# 免责说明

本程序仅供学习使用，禁止一切商业行为，如有法律责任，均和本程序作者无关，作者保留法律追究。
