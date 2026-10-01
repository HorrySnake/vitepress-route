# Route 静态网站

无需安装依赖或构建。将本目录内容上传到静态网站托管服务，并将本目录设置为网站根目录即可。

## 文件

- index.html：极简 App 落地页
- privacy.html：隐私说明
- terms.html：用户协议
- docs.html：文档概览
- docs/：保留原文档路径，兼容旧链接
- style.css：样式
- language.js：中英切换
- route-icon.png：正式产品图标

## 下载链接

首页下载按钮目前禁用。上线后，在 index.html 中将 button.download-pending 替换为链接，例如：

<a class="download-pending" href="你的 App Store 完整链接"><span lang="zh">在 App Store 下载</span><span lang="en">Download on the App Store</span></a>

并修改下方“开发中 · 即将上线”的文字。

## 隐私与协议

文档目前为开发阶段草案，正式使用前请核实产品的数据处理行为，并补齐运营主体、联系方式和生效日期。

## 托管注意

站内链接与资源路径已改为相对路径，兼容根目录及项目子目录托管。中英文内容使用 hidden 属性控制显示，默认中文。

该文件包不包含 Sites 配置、账户标识、Git 历史或访问凭据。网站没有依赖 Sites 的服务或 API。

## 本仓库部署

已替换原 VitePress 模板。`npm run build` 将上传的静态文件复制到 `dist/`，无需安装第三方依赖。保留 `edgeone.json` 的构建命令与输出目录，供已连接仓库的 EdgeOne Pages 自动部署。网站使用根目录链接，应部署到独立域名根目录。
