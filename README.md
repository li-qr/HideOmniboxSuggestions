# Hide Omnibox Suggestions

## 简介

Hide Omnibox Suggestions 是一个Chrome浏览器扩展程序,旨在提高用户的浏览隐私。它可以隐藏Chrome地址栏的搜索建议,并清理非白名单网站的浏览历史记录。

## 主要功能

- 自动隐藏地址栏搜索建议
- 支持白名单功能,允许特定网站不被清理历史记录
- 可以通过扩展图标快速将当前网站添加到白名单
- 在切换标签页时自动清理非白名单网站的历史记录
- 白名单支持正则表达式匹配

## 安装方法

1. 下载此仓库的ZIP文件并解压,或者使用git克隆此仓库。
2. 打开Chrome浏览器,进入`chrome://extensions/`页面。
3. 在右上角启用"开发者模式"。
4. 点击"加载已解压的扩展程序"按钮。
5. 选择包含扩展程序文件的文件夹。

## 使用方法

1. 安装后,扩展程序会自动隐藏所有网站的地址栏搜索建议。
2. 点击扩展程序图标可以快速将当前网站添加到白名单。
3. 在扩展程序的选项页面中,您可以手动添加、查看和删除白名单项目。
4. 白名单支持正则表达式,例如 `.*\.example\.com` 可以匹配所有 example.com 的子域名。
5. 每次切换标签页时,扩展程序会自动清理非白名单网站的历史记录。

## 文件结构

- `manifest.json`: 扩展程序的配置文件
- `background.js`: 后台脚本,处理历史记录清理等功能
- `content.js`: 内容脚本,用于隐藏地址栏搜索建议
- `popup.html` 和 `popup.js`: 扩展程序图标点击后的弹出页面
- `options.html` 和 `options.js`: 扩展程序的选项页面
- `icon.png`: 扩展程序图标

## 隐私声明

此扩展程序不会收集或传输任何用户数据。所有操作都在本地进行,包括白名单的存储和历史记录的清理。

## 贡献

欢迎提交 Issues 或 Pull Requests 来帮助改进这个项目。

## 许可证

MIT License
