# Mineradio

Mineradio-Kugou-Modified 是基于 Mineradio 的 Windows 桌面沉浸式音乐播放器修改版，在原有歌词舞台、粒子视觉、3D 歌单架和网易云 / QQ 音乐接入基础上，进一步加入酷狗音乐登录、云端歌单同步、用户信息同步和酷狗音源播放体验。

> **CodeEddie 二次维护版**
>
> 本仓库由 [CodeEddie](https://github.com/CodeEddie) 维护，自 2026-07-02 起基于
> [zws84952324-create/Mineradio-Kugou-Modified](https://github.com/zws84952324-create/Mineradio-Kugou-Modified)
> 进行二次创作，后续维护重点为界面视觉、交互细节与使用体验优化。本仓库不是上游项目的官方版本。

1.3.0 新增 Windows 动态壁纸库，内置极光脉冲、日蚀光环、黑胶唱片和星图连线四套模板；舞台歌词升级为当前句高亮、下一句弱化的双行显示，并支持调节未播放歌词透明度与歌词句间距。

## 当前版本

当前版本：`1.3.0`

状态：1.3.0 动态壁纸库与双行歌词正式版。

> 安全提示：`v1.0.10` 及更早旧安装包不再建议继续安装或传播，请先隔离旧安装包。本次不提供从 `v1.0.10` 到 `v1.1.0` 的软件内本地更新，请在 GitHub Release 页面手动下载 `v1.1.0` 安装包进行纯净安装。

## 下载与安装

[下载最新 Windows 安装包](https://github.com/CodeEddie/Mineradio-Kugou-CodeEddie/releases/latest/download/Mineradio-1.3.0-Setup.exe) · [下载免安装便携版](https://github.com/CodeEddie/Mineradio-Kugou-CodeEddie/releases/latest/download/Mineradio-1.3.0-Portable.zip) · [查看全部版本](https://github.com/CodeEddie/Mineradio-Kugou-CodeEddie/releases)

| 版本 | Windows 安装包 | 便携版 / 源码 | 更新说明 |
| --- | --- | --- | --- |
| `v1.3.0` | [下载安装包](https://github.com/CodeEddie/Mineradio-Kugou-CodeEddie/releases/download/v1.3.0/Mineradio-1.3.0-Setup.exe) | [便携 ZIP](https://github.com/CodeEddie/Mineradio-Kugou-CodeEddie/releases/download/v1.3.0/Mineradio-1.3.0-Portable.zip) | [Release](https://github.com/CodeEddie/Mineradio-Kugou-CodeEddie/releases/tag/v1.3.0) |
| `v1.2.0` | [下载安装包](https://github.com/CodeEddie/Mineradio-Kugou-CodeEddie/releases/download/v1.2.0/Mineradio-1.2.0-Setup.exe) | [便携 ZIP](https://github.com/CodeEddie/Mineradio-Kugou-CodeEddie/releases/download/v1.2.0/Mineradio-1.2.0-Portable.zip) | [Release](https://github.com/CodeEddie/Mineradio-Kugou-CodeEddie/releases/tag/v1.2.0) |
| `v1.1.3` | [下载安装包](https://github.com/CodeEddie/Mineradio-Kugou-CodeEddie/releases/download/v1.1.3/Mineradio-1.1.3-Setup.exe) | [便携 ZIP](https://github.com/CodeEddie/Mineradio-Kugou-CodeEddie/releases/download/v1.1.3/Mineradio-1.1.3-Portable.zip) | [Release](https://github.com/CodeEddie/Mineradio-Kugou-CodeEddie/releases/tag/v1.1.3) |

安装版：下载 `Setup.exe` 后双击安装，适合普通用户。便携版：解压完整 ZIP 后运行 `Mineradio.exe`，不要只复制单个 EXE。安装包暂未使用商业代码签名，Windows 可能显示“未知发布者”，请在本页核对 SHA256 后再运行。

> `dist/` 是本机构建目录，已被 `.gitignore` 排除，不会提交到 `main`。正式二进制统一托管在 GitHub Releases，避免每次发布都把数百 MB 文件永久写入 Git 历史。

## 核心特性

- Open-Meteo 实时天气与天气电台，根据当前位置快速显示天气、温度、体感和湿度，并生成更合适的播放队列
- 首页每日推荐支持网易云、QQ 音乐和酷狗音乐，可按全部来源或单个平台切换
- 首页六格支持右键移除，空位可通过加号恢复系统功能或固定个人云端歌单
- 首页每 30 秒从真实歌曲中随机读取一条热评，排除播客、本地文件和非歌曲记录
- Windows 动态壁纸库，支持极光脉冲、日蚀光环、黑胶唱片、星图连线四套模板及透明度调节
- 播放后切换到 Emily / 默认播放态视觉，歌词舞台与粒子舞台同步工作
- 基于节奏的电影镜头视觉系统
- 面向长播客和 DJ 曲目的专属视觉模式
- 双行歌词舞台：当前句高亮、下一句弱化，并支持未播放歌词透明度、歌词句间距、自定义歌词和布局控制
- 自定义专辑封面上传与裁剪
- 右键唤起 3D 歌单架，支持个人歌单与三平台每日推荐队列浏览
- 网易云音乐账号、搜索、歌单、播客等体验接入
- QQ 音乐搜索、网页登录态与音源补充接入
- 酷狗音乐网页登录、扫码登录、账号信息、VIP 状态、云端歌单、歌词和播放接口接入
- 网易云、QQ 音乐、酷狗支持优先音质与自动逐级降级，底部播放器显示实际音质和码率
- 默认播放软件支持 Mineradio、Windows 默认音频应用、自动识别网易云音乐和自选 EXE
- 三平台账号状态展示，已登录平台可在登录界面直接退出登录
- 首页空状态、登录弹窗、左侧歌单和底部播放控制栏视觉优化
- GitHub Releases 更新检测与下载入口
- 首次启动内置「默认测试」视觉用户存档，软件内默认视觉参数与该存档一致

## 使用说明

Windows 用户优先使用上方直链下载正式安装包。安装包会创建桌面快捷方式；便携版必须完整解压后再运行其中的 `Mineradio.exe`。

`v1.1.0` 不作为 `v1.0.10` 的软件内自动更新包发布。已经安装过旧版本的用户，建议卸载旧版本、隔离旧安装包后，再使用 `v1.1.0` 安装包纯净安装。

## 开发运行

```bash
npm install
npm start
```

桌面版入口由 Electron 主进程加载本地服务。

## 生成 Windows 安装包

环境要求：Windows 10/11、Node.js 20 或更新的 LTS 版本、npm。

```powershell
git clone https://github.com/CodeEddie/Mineradio-Kugou-CodeEddie.git
Set-Location Mineradio-Kugou-CodeEddie
npm install
node --check server.js
git diff --check
npm run build:win
```

构建完成后，`dist/` 中会生成：

- `Mineradio-x.y.z-Setup.exe`：Windows NSIS 安装包。
- `Mineradio-x.y.z-Setup.exe.blockmap`：软件更新差分信息。
- `latest.yml`：electron-updater 更新清单。
- `win-unpacked/`：未压缩的目录版，可用于本机验证或制作便携 ZIP。

只生成目录版、跳过安装器：

```powershell
npm run build:win:dir
```

制作便携 ZIP（把版本号替换为当前版本）：

```powershell
tar -a -cf dist/Mineradio-1.3.0-Portable.zip -C dist/win-unpacked .
```

生成 SHA256：

```powershell
Get-FileHash dist/Mineradio-1.3.0-Setup.exe -Algorithm SHA256
Get-FileHash dist/Mineradio-1.3.0-Portable.zip -Algorithm SHA256
```

仓库已配置 `.github/workflows/release.yml`。以后完成版本号和更新说明后，创建并推送版本标签即可自动构建并发布：

```powershell
git tag v1.3.0
git push origin v1.3.0
```

## 更新机制

Mineradio 会请求 GitHub Releases latest 检测新版本。远端版本高于本地版本时，应用内更新入口会展示 Release 内容、下载安装包到本机用户数据目录，并通过系统打开安装包。

本地验证更新链路时，可以通过 `MINERADIO_UPDATE_MANIFEST` 指向一个本地 manifest JSON 或 HTTP 地址来模拟线上 Release。

## 版本改动明细

完整原始记录见 [CHANGELOG.md](./CHANGELOG.md)。

<details open>
<summary><strong>v1.3.0 — 动态壁纸库与双行歌词</strong></summary>

- 正式开放 Windows 动态壁纸模式，视觉可挂载到桌面壁纸层。
- 新增极光脉冲、日蚀光环、黑胶唱片、星图连线四套模板。
- 壁纸模板、开关和透明度支持本地布局及用户存档。
- 舞台歌词升级为当前句高亮、下一句弱化的双行结构。
- 新增未播放歌词透明度与歌词句间距。
- 修复壁纸长时间运行后的亮度累积过曝。

</details>

<details open>
<summary><strong>v1.2.0 — 三平台每日推荐与可自定义首页</strong></summary>

- 每日推荐支持网易云、QQ 音乐和酷狗音乐。
- 支持全部来源或指定单个平台切换。
- 3D 歌单架新增每日推荐卡片及详情浏览。
- 首页六格改为可持久化槽位。
- 支持移除、恢复系统功能及固定个人云端歌单。
- 优化首页后台刷新，减少闪烁和交互中断。

</details>

<details open>
<summary><strong>v1.1.3 — 天气、热评、音质与外部播放器</strong></summary>

- 实时天气与天气电台拆分加载，城市天气显示更快。
- 热评严格排除播客、本地文件和非歌曲记录。
- 网易云、QQ、酷狗新增优先音质与逐级降级。
- 底部播放器显示实际音质和码率。
- 支持 Mineradio、Windows 默认应用、网易云和自选 EXE。
- 外部播放失败时自动回退 Mineradio。

</details>

<details>
<summary><strong>v1.1.1 — 安装器与卸载安全修复</strong></summary>

- 安装目录优先选择 D-Z 盘的独立 `Mineradio` 文件夹。
- 阻止安装到非空且不属于 Mineradio 的混合目录。
- 支持在安全的既有 Mineradio 目录中原位覆盖安装。
- 卸载器只删除已知程序文件，不再递归清空安装根目录。
- 跳过不可信的旧卸载器，避免间接触发旧版误删逻辑。

</details>

<details>
<summary><strong>v1.1.0 — 纯净重建与视觉系统稳定版</strong></summary>

- 从可信源码重新构建，隔离旧打包产物。
- 更新默认视觉存档和首次启动参数。
- 完善 3D 歌单架内容开关、镜头模式和详情页层级。
- 修复歌词与封面粒子世界轴、歌单详情页遮挡问题。
- 新增后台策略和低/中/高/超高画质档位。
- 修复应用视觉存档后切歌回退旧预设。
- 修复全屏控制台遮挡及更新失败循环。
- 更新 Electron 与 electron-builder 依赖。

</details>

<details>
<summary><strong>v1.0.10 — 桌面歌词与歌词布局</strong></summary>

- 重做桌面歌词白底可读性、长歌词滚动与锁定穿透。
- 修复安魂预设歌词位置和景深调节。
- 新增歌词上下角度、左右角度并持久化。
- 歌词镜头绑定时自动避让 3D 歌单架。
- 新增方向键音量调节并优化快速补丁规则。

</details>

<details>
<summary><strong>v1.0.9 — 安装体验与单实例</strong></summary>

- 安装器改为浅色高对比中文界面。
- 支持自由选择安装目录及盘符根目录自动补全。
- 应用改为单实例，重复启动会唤起现有窗口。
- 不再每次启动重复创建桌面快捷方式。

</details>

<details>
<summary><strong>v1.0.8 — QQ 授权、Home 与用户视觉存档</strong></summary>

- 修复 QQ 音乐账号资料与播放授权状态不同步。
- 调整 Home 入口和播放器控制台展开方式。
- 调整视觉预设顺序与安魂选中态。
- 新增四槽位视觉用户存档及命名。
- 修复歌词颜色恢复并增加播放暂停淡入淡出。

</details>

<details>
<summary><strong>v1.0.7 — 电影镜头与安魂预设</strong></summary>

- 调整电影镜头节奏分析。
- 完善安魂预设命名、卡片和自定义视觉染色。

</details>

<details>
<summary><strong>v1.0.6 — 开发中功能隔离</strong></summary>

- 将尚未稳定的桌面歌词、点击穿透和壁纸模式入口标记为开发中并关闭。

</details>

<details>
<summary><strong>v1.0.5 — 更新下载可靠性</strong></summary>

- GitHub 更新下载增加国内镜像与自动切换。
- 显示下载速度、大小、剩余时间和当前线路。
- 保留具体失败原因和尝试线路信息。
- 安装包与补丁增加 digest 校验。
- 收紧旧版本快速补丁匹配规则。

</details>

<details>
<summary><strong>v1.0.4 — 后台性能与控制台稳定性</strong></summary>

- 仅在真正最小化或隐藏时进入深度低占用。
- 修复全屏视觉画布裁切和偏移。
- 修复播放器控制台隐藏残影。
- 新增玻璃色差与视觉入口贴边隐藏。
- 左侧歌单详情改为分批加载。
- 恢复沉浸模式下歌单、歌单架和背景可用性。

</details>

<details>
<summary><strong>v1.0.3 — 视觉控制台重构</strong></summary>

- 控制台重构为预设、外观、歌词、动态、高级五个分区。
- 优化色轮和封面取色弹层定位。
- 区分纯黑背景与封面渐变模式。
- 保留并优化专辑封面背景取色。

</details>

<details>
<summary><strong>v1.0.2 — 歌曲操作与快速补丁</strong></summary>

- 艺术家详情歌曲新增收藏到歌单和下一首播放。
- 发布跨 `1.0.0`、`1.0.1` 的快速补丁与完整安装包。

</details>

<details>
<summary><strong>v1.0.1 — Emily 视觉过渡</strong></summary>

- 优化 Emily 视觉加载和切歌动画。
- 缩短封面颜色混合并让景深渐进淡入。
- 增加 `1.0.0 → 1.0.1` 快速补丁。

</details>

<details>
<summary><strong>v1.0.0 — 首个正式版本</strong></summary>

- 完成天气电台、每日推荐、继续听、听歌画像和歌单首页。
- 修复播放器控制台、进度条、播放暂停与切歌链路。
- 修复网易云、QQ 扫码登录状态落地。
- 隔离视觉、歌词、歌单架异常，避免阻断真实音频播放。
- 完善天气电台、歌单、播客和 3D 详情播放队列。
- 增加单曲循环、防递归和自动播放失败回退。
- 接入 Open-Meteo 并保持空闲星河与播放态视觉切换。

</details>

<details>
<summary><strong>v0.9.13 — 启动动画</strong></summary>

- 启动页升级为 WebGL 光流线场。
- 移除刻意爆点，改为自然斜向流线。
- 动画结束后等待用户点击或按键进入。
- 保留 2D Canvas 降级方案。

</details>

<details>
<summary><strong>v0.9.9 — 公开发布前整理</strong></summary>

- 统一版本号并接入 GitHub Releases 更新检测。
- 增加 QQ 音乐与网易云音乐双平台体验方向。
- 优化电影镜头节奏分析和 DJ 视觉。
- 增加封面、歌词、布局和视觉控制能力。

</details>

## 修改版说明

本仓库的二次维护关系如下：

1. 原始项目：[XxHuberrr/Mineradio](https://github.com/XxHuberrr/Mineradio)
2. 酷狗功能修改版：[zws84952324-create/Mineradio-Kugou-Modified](https://github.com/zws84952324-create/Mineradio-Kugou-Modified)
3. CodeEddie 二次视觉维护版：当前仓库

当前仓库继续遵循原项目 GPL-3.0 开源协议发布，主要进行界面视觉、交互细节和使用体验方面的二次更新。本修改版不代表原作者或上游维护者的官方版本，仅用于学习、研究和功能扩展练习。发布和分发时请保留原项目版权信息、`LICENSE`、`NOTICE.md` 等协议声明文件。

## 第三方音乐平台说明

Mineradio-Kugou-Modified 不是网易云音乐、QQ 音乐、酷狗音乐或腾讯音乐娱乐集团的官方客户端，也不隶属于任何音乐平台。

项目中的第三方平台接入仅用于个人学习、本地客户端体验和用户自有账号的播放辅助。请遵守对应平台的用户协议、版权规则和会员权益规则。项目不会提供绕过付费、绕过会员、破解音质或重新分发音乐内容的能力。

## 用户数据与隐私

登录 Cookie、搜索历史、自定义封面、自定义歌词、节奏分析缓存等数据只应保存在本机用户数据目录或浏览器本地存储中，不应提交到仓库。

更多说明见 [PRIVACY.md](./PRIVACY.md)。

## 作者支持

如果这个二次维护版对你有帮助，也欢迎支持 CodeEddie 继续进行视觉与交互更新。

[查看完整支持页](./docs/SUPPORT.md)

<p>
  <img src="./docs/assets/support/codeeddie-wechat-support.jpg" alt="CodeEddie 微信支持二维码" width="360">
  <img src="./docs/assets/support/codeeddie-alipay-support.jpg" alt="CodeEddie 支付宝支持二维码" width="360">
</p>

## 致谢

Mineradio 由 XxHuberrr 主要设计与打造。emily 作为早期视觉底层想法与 `emily` 视觉预设改进方向的共创者和灵感来源之一，特此感谢。

同时感谢小天才e宝、应春日、锋将军、軌跡、林中、骊、风痕、花椰菜🥦在早期体验、测试反馈和发布准备中的帮助。

## 版权与授权

Copyright (C) 2026 XxHuberrr.

本项目采用 GPL-3.0 授权。详见 [LICENSE](./LICENSE)。

MR Logo、Mineradio 名称、界面视觉设计与原创视觉表达归作者所有；第三方依赖和第三方服务分别遵循其各自授权与服务条款。
酷狗音乐相关功能用于用户自有账号的网页登录、歌单同步和播放体验测试，不提供破解会员、绕过版权限制、非法下载音乐等功能。第三方音乐平台名称和商标归其权利人所有，本项目与相关平台官方无从属、合作或授权关系。

---
