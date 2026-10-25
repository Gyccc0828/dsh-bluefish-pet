# 素材分发与版权归属

本项目分发软件代码、原版素材、衍生视频和历表数据。它们适用的许可不同；保留代码 MIT LICENSE 的同时，必须保留素材和数据的独立声明。下列内容是本分发版所用来源及处理方式的记录，不替任何原作者、商标权人或第三方新增授权。

## 1. 上游代码与原版素材

上游：[PC2005-cloud/dsh-pet](https://github.com/PC2005-cloud/dsh-pet)。本分发版基于其 0.3.7 安装版本，保留上游 Copyright (c) 2026 PC2005-cloud 的 [MIT 代码许可](LICENSE)。

原版动画、提示词和源视频的上游声明为允许开源使用、禁止商用，见 [上游 README 的许可段落](https://github.com/PC2005-cloud/dsh-pet#-许可)；本次检索时保存的上游提交参考为 `4eb75e6a5779ee7dccbed29dc83a621c1876d2f9`。原版视频没有因为被放进 npm 包而改为任意商用的 MIT 资源。

漫步复用原版踏步视频；奔跑、前扑摔倒、起身也来自原版完整视频，右向画面在播放时镜像。原文件及原始署名保留。字体、图标和表情包等其他上游资源保持各自既有权利和许可，本项目不为其增授权利。

## 2. Claude 卫衣与工作动作

来源：[lokicorvus / CrossPet 的 deepseek-hoodie](https://github.com/lokicorvus/crosspet/tree/6e98970f6ff9b44e8ac85215241cabcd78f67d92/characters/deepseek-hoodie)。[该提交的角色许可原文](https://github.com/lokicorvus/crosspet/blob/6e98970f6ff9b44e8ac85215241cabcd78f67d92/characters/LICENSE.md)为 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.zh-hans)。

按 CrossPet 的署名记录，角色原型「溟月」归因于 **上善无形**，深蓝鲸鱼女仆解释归因于 **ZipZipPipe**；本项目保留 CrossPet / lokicorvus 及这两位原作者的来源署名。

具体文件及改动：

- `变装-穿Claude衣服.webm`：以原版人物为形象参考、CrossPet 的卫衣为服装参考，使用 AI 辅助重绘并制作变装动画；该图不是 CrossPet 原图的无修改拷贝。
- `变装-Claude羽毛笔写字.webm`：使用该提交的 `writing.webp` 整张人物图，制作轻微上下浮动的透明视频。
- `变装-Claude左右递文件.webm`：使用 `busy_left.webp`、`busy_right.webp` 整张人物图，制作左右姿态轮换与轻微浮动。它不是连续手指打字动画。

这几项新增衍生画面／视频按 CC BY-NC-SA 4.0 分发，须署名、非商业使用，并对适用的衍生作品保留相同方式共享条件；底层角色及商标权利另行保留。完整上游原文见 [CLAUDE-WORK-SOURCE-LICENSE.md](third_party/CLAUDE-WORK-SOURCE-LICENSE.md)，逐项处理记录见 [CUSTOM-ASSETS-NOTICE.md](third_party/CUSTOM-ASSETS-NOTICE.md)。

## 3. 铁盆动作

`头顶铁盆-落下晃稳.webm` 的人物层连续使用 PC2005-cloud/dsh-pet 的原版待机视频。只有独立的深铁盆道具使用 AI 生成；道具落下、晃动和稳定由动画处理完成，没有直接拼入参考图片中的另一位人物。

铁盆外形参考：[Witherwithwinter / DeepSeek Balance Whale Widget Bowl](https://github.com/Witherwithwinter/DeepSeek-Balance-Whale-Widget-Bowl/tree/2154a5deb30039f9f5825677b653a825975fcee2)，参考图片为 `assets/DSniang-bowl.png`。其 MIT 声明保留 Copyright (c) 2026 MeteorNOX 与 Copyright (c) 2026 Witherwithwinter，全文见 [BASIN-SOURCE-LICENSE.txt](third_party/BASIN-SOURCE-LICENSE.txt)。人物动画和角色权利另按原版素材来源保留。

新增铁盆衍生画面／视频按 CC BY-NC-SA 4.0 提供，受底层角色／动画的适用权利约束；不将 AI 辅助生成描述为对原角色的独占版权。详见同目录素材处理记录。

## 4. 历表数据

数据来源：[香港天文台公历与农历对照表](https://www.hko.gov.hk/en/gts/time/conversion.htm)、[DATA.GOV.HK 历表数据集](https://data.gov.hk/en-data/dataset/hk-hko-rss-gregorian-lunar-calendar-conversion-table)。数据归属署名：**香港特别行政区政府／香港天文台**，并注明 **DATA.GOV.HK** 来源。

本版提取 2020—2100 年相应农历节日和节气日期，保留来源及其 [数据使用条款](https://data.gov.hk/en/terms-and-conditions)。本地的动作对应关系和前后七天窗口为本项目安排，不代表数据提供方对桌宠产品的认可。详见 [SEASONAL-CALENDAR-SOURCE.md](third_party/SEASONAL-CALENDAR-SOURCE.md)。

## 5. 再分发时需要保留什么

1. 原代码 MIT 许可全文及版权声明，以及本 NOTICE 和各项素材／数据来源链接。
2. CrossPet、上善无形、ZipZipPipe 等来源署名，CC BY-NC-SA 4.0 链接及素材改动标记。
3. 非商业限制和适用衍生作品的相同方式共享条件，不把含这些素材的整包标为任意商用的纯 MIT 包。
4. 铁盆参考项目的原始 MIT 说明，以及历表数据的提供方和 DATA.GOV.HK 署名。

本项目为非官方同人定制。DeepSeek、Claude 等名称与商标归各自权利人；新增代码、整理打包或 AI 辅助处理均不会取消底层角色和素材的权利。若权利人对具体使用有异议，可在本仓库提 Issue，以便核实并更正或移除相关内容。
