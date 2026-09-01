> [!TIP]
> **JJC 定制版** - 同步自 automa/AutomaApp，qmhdl1027 维护

<img src="src/assets/images/icon-128.png" width="64"/>

# Automa
<p>
  <img alt="Automa 最新版本" src="https://img.shields.io/github/package-json/v/AutomaApp/automa" />
  <a href="https://twitter.com/AutomaApp">
    <img alt="在 Twitter 上关注我们" src="https://img.shields.io/twitter/follow/AutomaApp?style=social" />
  </a>
  <a href="https://discord.gg/C6khwwTE84">
    <img alt="在 Discord 上与我们交流" src="https://img.shields.io/discord/942211415517835354?label=join%20discord&logo=Discord&logoColor=white" />
  </a>
</p>

> [!TIP]
> 🚀 **JJC 定制版** — 同步自 automa/AutomaApp，浏览器自动化扩展中文版

一个通过连接模块（Blocks）来自动化浏览器操作的 Chrome 扩展。<br />
自动填写表单、执行重复性任务、截图、爬取网页数据 —— 由你决定。你还可以设置定时任务，自动执行自动化流程！

## 📥 下载

<table cellspacing="0" cellpadding="0">
  <tr>
    <td valign="center">
      <a align="center" href="https://chrome.google.com/webstore/detail/automa/infppggnoaenmfagbfknfkancpbljcca">
        <img src="https://user-images.githubusercontent.com/22908993/166417152-f870bfbd-1770-4c28-b69d-a7303aebc9a6.png" alt="Chrome 网上应用店" />
        <p align="center">Chrome 网上应用店</p>
      </a>
    </td>
    <td valign="center">
      <a href="https://addons.mozilla.org/en-US/firefox/addon/automa/">
        <img src="https://user-images.githubusercontent.com/22908993/166417727-3481fef4-00e5-4cf0-bb03-27fb880d993c.png" alt="Firefox 附加组件" />
        <p align="center">Firefox 附加组件</p>
      </a>
    </td>
  </tr>
</table>

## 🎯 功能特性

- **🌐 浏览器自动化** — 自动点击、填写表单、导航页面、截取截图等
- **📋 工作流设计器** — 可视化拖拽连接 Blocks，构建复杂自动化流程
- **🕸️ 网页数据爬取** — 从任意网站提取结构化数据
- **⏰ 定时任务** — 设置何时自动执行自动化流程
- **📦 扩展构建器** — 将工作流导出为独立的 Chrome 扩展
- **🔌 丰富模块** — 支持循环、条件判断、JS 代码执行、数据存储等
- **💾 数据存储** — 内置数据存储，支持 JSON/CSV 导出

## 🛒 插件市场

在 Automa 插件市场浏览和下载其他用户分享的工作流。[前往插件市场 &raquo;](https://extension.automa.site/marketplace)

## 🔧 Automa Chrome 扩展构建器

Automa Chrome 扩展构建器（Automa CEB）可以将你的工作流生成为一个独立的 Chrome 扩展，方便分发和部署。[查看文档 &raquo;](https://docs.extension.automa.site/extension-builder)

## 🚀 快速开始

### 1. 安装扩展

#### Chrome
1. 打开 Chrome，访问扩展管理页面：`chrome://extensions`
2. 开启右上角的「**开发者模式**」
3. 点击「**加载已解压的扩展程序**」按钮，选择 `automa/build` 目录

![在 Chrome 中安装](https://user-images.githubusercontent.com/22908993/166417152-f870bfbd-1770-4c28-b69d-a7303aebc9a6.png)

#### Firefox
1. 打开 Firefox，访问 `about:debugging#/runtime/this-firefox`
2. 点击「**加载临时附加组件**」按钮
3. 浏览到 `automa/build` 目录，选择 `manifest.json` 文件

![在 Firefox 中安装](https://user-images.githubusercontent.com/22908993/166417727-3481fef4-00e5-4cf0-bb03-27fb880d993c.png)

### 2. 创建你的第一个自动化流程

1. 点击扩展图标打开 Automa 界面
2. 点击「**新建工作流**」
3. 从左侧面板拖拽 Blocks 到画布区域
4. 连接各模块，配置参数
5. 点击「**测试运行**」验证流程
6. 满意后保存，绑定快捷键或定时执行

### 3. 编译打包（可选）

如需从源码编译，先创建 `src/utils/getPassKey.js`：

```js
export default function() {
  return '任意字符串';
}
```

然后运行以下命令：

```bash
# 安装依赖
pnpm install

# Chrome 开发模式（热重载）
pnpm dev

# 编译生产版本（Chrome）
pnpm build

# 打包为 zip 文件
pnpm build:zip

# Firefox 开发模式
pnpm dev:firefox

# 编译生产版本（Firefox）
pnpm build:firefox

# 代码检查与修复
pnpm lint
```

#### 图标预览
v-remixicon/icons: https://preview-v-remixicon.vercel.app/

## 📚 相关资源

- 📖 [官方文档](https://docs.extension.automa.site/)
- 🏪 [插件市场](https://extension.automa.site/marketplace)
- 🐦 [Twitter](https://twitter.com/AutomaApp)
- 💬 [Discord 社区](https://discord.gg/C6khwwTE84)

## 🤝 贡献者

感谢所有提交问题、提出建议的朋友，让 Automa 变得更好！

<a href="https://github.com/AutomaApp/automa/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=AutomaApp/automa" />
</a>

## 📄 开源许可

本仓库源代码采用 [GNU Affero General Public License v3 (AGPL-3.0)](https://www.gnu.org/licenses/agpl-3.0.html) 或 [Automa 商业许可](https://extension.automa.site/license/commercial/) 双许可。

详情请参阅 [LICENSE.txt](./LICENSE.txt)。
