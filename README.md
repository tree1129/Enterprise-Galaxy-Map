# Enterprise Galaxy Map｜企业星图

面向硬科技与 AI 企业的交互式企业星系演示。项目通过空间点云、产业分类、企业画像和关系连线，将企业能力、上下游关系与 AI 自动化服务放在同一个可视化界面中。

## 在线体验

- GitHub Pages：<https://tree1129.github.io/Enterprise-Galaxy-Map/>
- Sites 版本：<https://hardtech-enterprise-galaxy-cn.sure-quail-6882.chatgpt.site/>

## 当前功能

- 116 家硬科技与 AI 企业的空间星系展示
- 按产业分类筛选与企业搜索
- 企业详情、能力方向和合作需求画像
- 企业关系连线与重点关系高亮
- “建立我的星系图”与手动联系
- AI 自动推荐潜在合作关系
- 企业内部 AI Todo 与人机协作流程演示
- 响应式桌面与移动端布局

## 项目结构

```text
.
├── dist/
│   ├── .nojekyll
│   └── index.html          # 完整静态网页
├── .github/workflows/
│   └── pages.yml           # GitHub Pages 自动部署
└── README.md
```

## 本地运行

这是一个无构建依赖的静态网页，可以直接打开 `dist/index.html`，也可以启动本地静态服务器：

```bash
python3 -m http.server 8080 --directory dist
```

然后访问 <http://localhost:8080>。

## 数据说明

当前企业信息和关系主要用于产品原型演示。正式产品接入企查查、IT 桔子、政府公开数据或企业内部数据时，需要取得相应授权，并保留数据来源、更新时间、证据和纠错机制。

## 部署

推送到 `main` 分支后，GitHub Actions 会自动将 `dist` 目录发布到 GitHub Pages。

