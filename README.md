# 分批加仓跟踪（浏览器单页）

本地数据、自选多股、行情与 K 线、计划表与新闻等均在单文件 `index.html` 中运行，无需构建。

## 使用方式

1. 克隆本仓库后，用浏览器直接打开根目录下的 **`index.html`**；或  
2. 开启 **GitHub Pages**（仓库 Settings → Pages → Branch 选 `main`、文件夹选 `/ (root)`），通过站点地址访问。

上一版纯手动界面见同目录 **`stock-strategy-tracker-classic.html`**（页面内也有入口链接）。

## 上传到 GitHub（示例）

在**本文件夹**内执行：

```bash
git init
git add .
git commit -m "Initial commit: stock strategy tracker"
```

在 GitHub 新建空仓库后：

```bash
git remote add origin https://github.com/<你的用户名>/<仓库名>.git
git branch -M main
git push -u origin main
```

## 说明

- 数据保存在浏览器 **localStorage**，换设备或清除站点数据后需重新录入。  
- 行情与 K 线依赖外网脚本与接口；若部署在 GitHub Pages，请留意浏览器跨域与混合内容策略。
