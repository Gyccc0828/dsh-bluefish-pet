# dsh-bluefish-pet 分发包

这是一个基于 `dsh-pet` 的 DeepSeek Harness 桌面宠物分发包，默认显示蓝色大肥鱼。它适用于 DSH Desktop 的桌面模式，也可以在 web profile 中安装后使用网页半侧功能。

## 功能

- 透明桌面窗口，支持待机、工作状态和点击动画
- 左键点击桌宠时刷新 DeepSeek 余额，并显示余额气泡
- 右键菜单提供“桌宠缩放”，支持 50%、75%、100%、125%、150% 和 200% 等比例
- 右键菜单提供“退出桌宠”，只关闭桌宠窗口，不退出 DSH
- 缩放比例保存在 `$DSH_HOME/dsh-pet/desktop-scale.json`，重启桌面模式后仍会保留
- 余额请求在 DSH Host 侧完成，不把 API Key 交给浏览器
- 默认关闭自动碎碎念，避免后台模型调用

## 桌宠怎么操作

启动 DSH Desktop 并启用本插件后，桌宠会自动出现在桌面上。右键点击桌宠：

- 选择“桌宠缩放”即可按比例调整大小
- 选择“退出桌宠”即可关闭桌宠窗口

退出后，重新启用插件、修改桌宠配置或重启 DSH Desktop 即可再次启动桌宠。

## 用 DSH 插件管理页安装

打开 DSH Desktop → Settings → Plugins，在本地包安装入口选择这个 `.tgz` 文件，然后重启 DSH Desktop。

如果已经安装官方 `dsh-pet`，先移除旧包再安装本包，避免两个插件同时创建桌宠：

```powershell
dsh plugin --profile desktop remove dsh-pet
```

然后安装本包：

```powershell
dsh plugin --profile desktop add .\dsh-bluefish-pet-0.1.0.tgz
```

首次桌面模式可能自动下载 Electron 运行时。点击余额前，请先在 DSH 中配置 DeepSeek API Key，或登录 DSH 的 DeepSeek 账号。

## 用命令行安装

```powershell
# desktop profile
dsh plugin --profile desktop add .\dsh-bluefish-pet-0.1.0.tgz

# 或 web profile
dsh plugin --profile web add .\dsh-bluefish-pet-0.1.0.tgz
```

## 许可和署名

本包保留上游 `PC2005-cloud/dsh-pet` 的 MIT 代码许可和原始署名。上游动画、提示词和源视频遵循上游仓库的素材条款：允许开源使用，禁止商用；二次分发时请保留原作者链接。

上游项目：[PC2005-cloud/dsh-pet](https://github.com/PC2005-cloud/dsh-pet)

