# Route 静态网站

纯 HTML、CSS、JavaScript，无框架和安装依赖。

## GitHub Pages

Settings → Pages → Source 选择 **GitHub Actions**。推送 main 后自动发布。默认网址为 https://horrysnake.github.io/vitepress-route/ 。站内链接为相对路径，兼容项目子目录。私有仓库使用 Pages 需要账户套餐支持；部署不会改变仓库可见性。

也可以选择 Deploy from a branch，使用 main / (root) 直接发布。自动工作流方案则使用 GitHub Actions 来源。

## 本地预览

在仓库目录运行 `python3 -m http.server 8082`。

## 内容

首页 index.html，隐私说明 privacy.html，用户协议 terms.html，文档概览 docs.html。docs/ 保留兼容路径。language.js 管理中英文切换。

下载按钮当前禁用，App 上线后填写实际 App Store 链接。法律文本仍为开发阶段草案，正式发布前需确认运营主体、联系方式及实际数据处理行为。
