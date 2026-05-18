# 原油基本性质查询

这是一个静态网页，可以部署到 Vercel、GitHub Pages 或任意静态网站托管服务。页面数据来自 `原油基本性质201505.xls`，支持按中文名称、英文名称进行模糊检索，并可按产地和原油类别筛选。

公网地址：

https://zyb0716-svg.github.io/crude-oil-query-site/

## 重新生成数据

```powershell
py -3 .\scripts\extract_data.py "<原油基本性质201505.xls 的路径>" .\assets\data.js
```

## 部署到 Vercel

```powershell
vercel --prod
```

在 Vercel 上选择当前目录作为项目根目录即可。
