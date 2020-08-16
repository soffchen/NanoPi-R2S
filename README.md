# 使用 Github Actions 在线编译 NanoPi-R2S 固件

* NanoPi R2S CNC 官方金属壳版 购买链接: [https://s.click.taobao.com/ZPSFRyu](https://s.click.taobao.com/ZPSFRyu) 

## 说明
* 管理 IP: 192.168.2.1
* 默认管理密码: password

## 特色
* 支持 RTL8821CU/RTL8822BU 芯片的 USB WiFi 设备，已知支持列表：
    - [COMFAST 726B](https://u.jd.com/KmtGTP)
    - [COMFAST CF-759BF](https://u.jd.com/AiZit7)
* 集成 [frainzy1477/luci-app-clash](https://github.com/frainzy1477/luci-app-clash) 及其 clash bin（CONFIG_PACKAGE_luci-app-clash 默认没开启）
* 集成 [vernesong/OpenClash](https://github.com/vernesong/OpenClash) 及其 clash bin
* 集成 [rufengsuixing/luci-app-adguardhome](https://github.com/rufengsuixing/luci-app-adguardhome)
* 集成 [coolsnowwolf/packages](https://github.com/coolsnowwolf/packages), [coolsnowwolf/luci](https://github.com/coolsnowwolf/luci) 与 [coolsnowwolf/lede/package/lean](https://github.com/coolsnowwolf/lede/tree/master/package/lean)
* 更新 [jerrykuku/luci-theme-argon](https://github.com/jerrykuku/luci-theme-argon)
* 集成 [songchenwen/nanopi-r2s/luci-app-r2sflasher](https://github.com/songchenwen/nanopi-r2s/tree/master/luci-app-r2sflasher)
* 集成 [pymumu/smartdns](https://github.com/pymumu/smartdns) 与 luci-app-smartdns
* 集成 [luci-app-oled](https://github.com/NateLol/luci-app-oled)
* 集成 [luci-app-jd-dailybonus](https://github.com/jerrykuku/luci-app-jd-dailybonus)

## 用法
Fork 到自己的账号下，将 `.github/workflows` 下 `.yml` 文件中的 `runs-on: self-hosted` 改成 `runs-on: ubuntu-latest`（因为我是自己的服务器上编译，更快），编辑文件 `CHANGELOG.md` 触发编译动作。

## 注意
产品发布初期，官方代码每天都在变，遇到无法编译时，请过来查看 `.yml` 与 `config` 最新异动。

## 参考
* [使用Github的Actions功能在线编译NanoPi-R1S固件（包含H5和H3）](https://totoro.site/index.php/archives/70/)
* [skytotwo/NanoPi-R1S-Build-By-Actions](https://github.com/skytotwo/NanoPi-R1S-Build-By-Actions)
* [klever1988/nanopi-openwrt](https://github.com/klever1988/nanopi-openwrt)
* [yangliu/NanoPi-R2S](https://github.com/yangliu/NanoPi-R2S)
* [maxming2333/NanoPi-R2S](https://github.com/maxming2333/NanoPi-R2S)
* [songchenwen/nanopi-r2s](https://github.com/songchenwen/nanopi-r2s)
* [fanck0605/nanopi_r2s](https://github.com/fanck0605/nanopi_r2s)
