# ChemDB Atlas · 计算化学资源导航

将用户提供的“讲解版源文件”和“chemdb-agent”制作成响应式中文网页。

- 103 条完整资源目录、11 个主题；支持搜索、筛选、收藏、详情和 CSV 导出。
- 19 页讲解全文，支持章节跳转、手机阅读与当前章节打印。
- Agent 实际进度、任务选库路径、本地运行示例及原项目源码下载。
- 无外部字体、统计服务或前端依赖，可离线打开 `dist/index.html`。
- 收藏保存在当前浏览器。网页不执行化学数据库 API 查询，不收集 API key。

## 源材料与边界

内容来自用户提供的 2026-10-27 成果包。资源网站地址和端点状态是材料记录，制作网页时没有重新进行外部 API 验证。

已存在 9 个数据源接入模块，不等于所有 MCP 查询工具可用。原源码的 `search_structures`、`get_record`、`search_molecules`、`get_basis` 等仍返回占位状态；网页明确展示这一边界。

## 本地预览

在本目录运行 `python -m http.server 4173 --directory dist`，然后访问 `http://localhost:4173`。也可直接双击 `dist/index.html`。

## GitHub Pages

`.github/workflows/pages.yml` 已配置发布 `dist/`。在 GitHub 仓库设置的 Pages 中选择 GitHub Actions，即可在推送后部署。仓库是否公开由用户决定。
