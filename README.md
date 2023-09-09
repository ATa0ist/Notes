# NOTEBOOK

## 笔记

## 问题&解决办法  

- ###  http自动跳到https  

  - 点击地址栏左侧不安全警告，启用警告

- ###  git 回滚到某个版本并删除提交记录  

  - ```bash
          git reset --hard a6sd485(版本号)
          git push -f origin(本地分支名称) main(远程分支名称)
    ```

- ###  google 设备认证 SafetyNet认证 失效

     1. magisk 把root对谷歌服务、商店等隐藏
     2. 安装 [Universal SafetyNet Fix](https://github.com/kdrag0n/safetynet-fix) 或 [Universal SafetyNet Fix[MOD]](https://github.com/Displax/safetynet-fix) 模块(最近我系统更新后用原版的失效了，换了mod版后恢复了)
     3. **飞行模式**下多清空几次 play商店 和 play服务 的数据，然后重启之后再打开网络

- ###  开启OpenClash后dns解析失败,关闭后恢复正常

  - 提示"找不到xxx.xxx的服务器IP地址"或"找不到xxx.xxx的DNS地址"
     1. 覆写设置→dns设置→勾选 自定义上游 DNS 服务器，然后在下面fallback组里多勾个1.1.1.1 8.8.8.8啥的

     2. _[不推荐]插件设置→dns设置→本地DNS劫持→使用 Dnsmasq 转发，改成【停止/防火墙】_

- ###  Openwrt下dnsmasq强行清理某个DHCP租约

     1. 编辑 `/tmp/dhcp.leases` 文件，删除想清理的IP地址/MAC地址那一行
     2. 重启dnsmasq：`/etc/init.d/dnsmasq restart`
     3. PC上：`ipconfig /release` 或 断网重连

- ###  应用分身文件路径

  - /storage/emulated/999/

- ###  卸载7zip后打开方式还在

  - 注册表 `HKEY_CLASSES_ROOT\Applications` 里删除相关项目

## 思考

## IDEA
