# dsh-bluefish-pet · 蓝色大肥鱼桌宠分发版

基于 [PC2005-cloud/dsh-pet](https://github.com/PC2005-cloud/dsh-pet) 0.3.7 的非官方定制分发版，适用于 DeepSeek Harness。项目负责定制动作、配置和打包，原作者、上游代码、角色素材及第三方数据的权利分别保留。

**当前版本：`0.3.7-bluefish.20261025.1`** · [下载可移植安装包](<https://github.com/Gyccc0828/dsh-bluefish-pet/releases/download/v0.3.7-bluefish.20261025.1/dsh-pet-0.3.7-bluefish.20261025.1.tgz>) · [发布说明](https://github.com/Gyccc0828/dsh-bluefish-pet/releases/tag/v0.3.7-bluefish.20261025.1) · [SHA-256 校验](SHA256SUMS.txt)

> 代码采用 MIT；随包角色及衍生素材含非商业使用和相同方式共享要求。不能把代码的 MIT 许可套用到全部角色素材。分发前请阅读 [素材分发与版权归属](ASSET_LICENSES.md) 和 [NOTICE](NOTICE.md)。

## 本版功能与更新

- 移动动作精简为 **漫步、原地左转奔跑、原地右转奔跑**；左右奔跑保留原版“起跑 → 前扑摔倒 → 起身”，向右动作由播放器镜像，跑动时沿对应方向移动。移除螃蟹走路、左右漫步入口。
- 保留基础 Claude 卫衣变装，加入 **Claude 羽毛笔写字、左右递文件**。两项工作动作参与工作状态联动，待机概率为 **0**，仍可在「动作 → Claude工作」手动点播。
- 铁盆从上方落下，左右晃动后稳住；盆为 **大而深、扣在额前** 的样式，人物连续使用原版形象。旧敲盆回弹和钢管动作移除。
- **21 个时节动作**仅在相关节日／节气前后各 **7 天**自动触发，包含当天和两端日期；全年可手动点播。农历、节气按逐年离线历表判断，覆盖 2020—2100 年。
- 保留桌宠右键菜单的查看余额、比例缩放和退出桌宠，以及原有点击／拖拽、工作状态功能。

完整更新见 [CHANGELOG](CHANGELOG.md)，时节对应关系见 [日期对照表](docs/seasonal-actions.md)。

## 安装或升级

1. 下载本版 `.tgz`，无需解压。
2. 在 DSH Desktop 的设置 → 插件中使用本地包安装入口选择它，随后重启 DSH Desktop。
3. 若使用命令行，选择当前 DSH 自带／对应的 CLI：

```powershell
dsh plugin --profile desktop add .\dsh-pet-0.3.7-bluefish.20261025.1.tgz
```

网页模式改用 `--profile web`。本版安装名称仍为 **`dsh-pet`**，仓库名称是 `dsh-bluefish-pet`；若安装过旧分发版 `dsh-bluefish-pet`，先停用或移除旧包，避免重复桌宠。

已有 `dsh-pet` 时以同名包更新；个人配置继续保留。目标机器自定义的完整 `animations` 段会覆盖新默认动作，更新后需要检查这一项。详细步骤见 [安装说明](docs/INSTALL.md)。

本包提供代码、素材、字体、图标和离线历表，不带个人设置、聊天记录、账号或 API Key。首次安装／启动可能下载依赖和 Electron。包内默认配置开启自动碎碎念（会使用当前模型），可在设置里关闭；目标机器已有设置不会被分发包强制覆盖。

## 版本与验证范围

本版为已构建分发包；运行代码、默认动作配置和素材来自当前已验证的定制版本，只调整分发元数据和说明文档。

- 328 个文件校验及换目录解压检查通过；111 个菜单动作均能找到随包素材。
- 换目录后 DSH 插件元数据、图标和声明兼容性检查通过，移动菜单、时节筛选和 Claude 待机排除保留。
- 保留上游 Node.js `>=22.12.0` 和 DSH 0.2.0-rc.1／0.2.0-rc.2 的兼容性声明；其他版本及另一台电脑上的完整启动没有新增验证。
- WebM 透明视频适合 Chromium／Electron；本包不包含 Safari 所需的 MOV 素材。

大安装包通过 GitHub Releases 附件分发，源码和构建产物均在 `.tgz` 的 `package/src`、`package/lib` 中。此仓库保存分发文档、许可和校验信息，不把视频包提交到 Git 历史。旧 [v0.1.0 发布](https://github.com/Gyccc0828/dsh-bluefish-pet/releases/tag/v0.1.0) 保留。

## 来源与许可

| 内容 | 来源／归属 | 适用说明 |
|---|---|---|
| 插件代码 | PC2005-cloud/dsh-pet 及本项目定制修改 | [MIT 代码许可](LICENSE)，保留版权声明 |
| 原版动画、提示词、源视频 | PC2005-cloud/dsh-pet | 上游声明允许开源使用、禁止商用；不以代码 MIT 覆盖素材条款 |
| 角色原型及蓝鲸女仆设定 | 按 CrossPet 署名：上善无形（溟月）、ZipZipPipe（蓝鲸女仆解释） | 原作者及底层权利保留，见 [详细署名](ASSET_LICENSES.md) |
| Claude 参考与两项工作素材 | lokicorvus / CrossPet | CC BY-NC-SA 4.0，保留署名、非商业和相同方式共享要求 |
| 铁盆外形参考 | Witherwithwinter / DeepSeek Balance Whale Widget Bowl | 保留参考项目 MIT 声明；人物权利另依原版素材条款 |
| 节日／节气历表 | 香港特别行政区政府／香港天文台，经 DATA.GOV.HK 提供 | 按数据使用条款保留来源和归属 |

基础 Claude 卫衣图和独立盆道具使用 AI 辅助生成／编辑，工作动作则基于 CrossPet 完整人物图转制；这些处理不抹去底层素材权利。项目为非官方同人定制，与相关品牌公司及数据提供方无隶属或背书关系。
