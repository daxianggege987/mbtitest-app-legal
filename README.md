# 人格图鉴 PersonaAtlas · 隐私政策与技术支持（静态页）

本仓库**仅**托管 App Store 所需的 **`privacy.html`** 与 **`support.html`**，通过 GitHub Pages 提供 HTTPS 链接。不包含 iOS 应用源代码。

## 线上地址

- 入口页：https://daxianggege987.github.io/mbtitest-app-legal/
- **隐私政策**：https://daxianggege987.github.io/mbtitest-app-legal/privacy.html
- **技术支持**：https://daxianggege987.github.io/mbtitest-app-legal/support.html

App Store Connect 里「隐私政策网址」填上面的 privacy 链接，「技术支持网址」填 support 链接。各语言本地化可填写**同一 URL**，用户打开后自行切换语言。

## 中英双语

两个页面右上角均有 `中文 / EN` 切换：

- 默认跟随浏览器语言（`zh*` → 中文，其余 → 英文）；
- 手动选择会保存到 `localStorage`，下次访问自动恢复；
- 也支持 URL 指定：`privacy.html?lang=en`（便于在 App Store 各语言本地化里分别填入对应语言）。

切换时同步更新页面标题、`<html lang>` 与按钮状态，无整页刷新。

## 文件

| 说明 | 路径 |
|------|------|
| 入口页 | `docs/index.html` |
| 隐私政策 | `docs/privacy.html` |
| 技术支持 | `docs/support.html` |

页面均为单文件自包含（CSS/JS 内联），无外部依赖、无第三方字体与统计脚本，可离线打开。

## 修改方式

1. 编辑 `docs/` 下的 HTML；
2. `git add -A && git commit -m "update" && git push origin main`；
3. GitHub Pages 通常 1 分钟内刷新（可用 `gh api repos/daxianggege987/mbtitest-app-legal/pages/builds/latest` 查看状态）。

修改隐私政策内容时，请同步更新两个语言版本，并改文首的生效日期。

## 与应用内事实保持一致

以下内容如与应用实际行为不符，请同步修改页面，否则会有审核风险：

- 广告服务为 **Google AdMob**（横幅 / 插页 / 激励视频 / 原生）；
- 应用**无账号、无服务器**，答题与结果仅存本机；
- 当前**未接入任何第三方统计分析服务**——若将来接入，需更新第 5 节并同步修改 App Store 隐私标签；
- 应用不面向 13 岁以下儿童，不含内购与社交功能。
