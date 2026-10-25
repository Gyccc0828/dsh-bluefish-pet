# 可移植安装说明

文件：`dsh-pet-0.3.7-bluefish.20261025.1.tgz`。这是可直接安装的 npm 格式插件包，内部安装名称仍为 `dsh-pet`。保留这个名称是为了与 DSH 的插件入口、已有配置和素材加载路径一致。项目仓库名仍为 `dsh-bluefish-pet`。

## 安装到另一套 DSH

将 `.tgz` 复制到目标电脑。在 DSH Desktop 的设置 → 插件中，通过本地包入口选择该文件，然后重启 DSH Desktop。也可在能使用 `dsh` 命令的终端执行：

```powershell
dsh plugin --profile desktop add .\dsh-pet-0.3.7-bluefish.20261025.1.tgz
```

网页模式对应：

```powershell
dsh plugin --profile web add .\dsh-pet-0.3.7-bluefish.20261025.1.tgz
```

使用绝对路径时给路径加引号。不需要先解压 `.tgz`。

若目标 DSH 之前安装的是本仓库旧的 `dsh-bluefish-pet` 包，先停用或移除那个旧包，再安装本次 `dsh-pet`，避免创建两只重复桌宠。目标机器已有 `dsh-pet` 时使用同名包更新，并保留自己的设置；旧用户配置中的完整 `animations` 段会覆盖新默认动作，需要备份后在设置中检查这一项。

## 包含与运行条件

- 插件代码、透明 WebM、字体、图标、表情包、离线节日历表和素材署名均已包含；无本机绝对路径依赖。
- 不包含个人用户设置、聊天记录、API Key、DSH 账号、Electron 可执行程序或 DSH 主程序。
- 插件依赖由目标 DSH 的包管理器安装；桌面模式首次使用可能下载 Electron，因此首次安装／首次启动不保证完全离线。
- 声明的 Node.js 要求为 `>=22.12.0`；保留上游 DSH 兼容性声明（0.2.0-rc.1、0.2.0-rc.2）。其他 DSH 版本和跨操作系统实际启动尚未验证。
- 透明 WebM 适用于 Chromium／Electron。Safari 的透明视频兼容问题沿用上游限制；本包不含 MOV 素材。
- 包内默认配置显示网页和桌面两种形态，工作状态联动开启、固定模式关闭；自动碎碎念默认开启，会使用当前模型，可在桌宠设置中关闭。

本包复制当前已验证的插件配置，不覆盖目标电脑的个人配置。安装后可在「动作 → 移动」检查漫步、原地左转奔跑、原地右转奔跑，在「动作 → Claude工作」检查两个工作动作。

## 许可

软件代码保留 MIT；原版及衍生角色素材按其各自许可保留署名和非商业限制，其中 CrossPet／Claude 衍生素材为 CC BY-NC-SA 4.0。历表数据署名香港特别行政区政府／香港天文台。完整说明见随包 `CUSTOM-ASSETS-NOTICE.md`、`CLAUDE-WORK-SOURCE-LICENSE.md`、`BASIN-SOURCE-LICENSE.txt`、`SEASONAL-CALENDAR-SOURCE.md`。本包不改变任何原有素材权利。
