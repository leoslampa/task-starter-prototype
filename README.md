# 一句话任务启动助手

一个面向项目负责人的静态网页工具，用于把一句模糊任务快速转成任务启动小报告。

核心流程：

- 三思：形成项目负责人当前理解、任务边界、偏航风险、任务拆解。
- 慎问：生成 3-5 个关键待确认事项、询问对象和建议问法。
- 留痕：记录原始任务原话和待确认事项。

## 试用方式

直接打开 `index.html` 即可本地试用。

## 公网部署

这是纯前端静态站点，可部署到：

- Vercel
- Netlify
- Cloudflare Pages
- GitHub Pages

部署时只需要发布当前目录即可。

### GitHub Pages 发布方式

1. 在 GitHub 新建一个公开仓库，例如 `task-starter-prototype`。
2. 将本地代码推送到仓库的 `main` 分支。
3. 进入仓库 `Settings` -> `Pages`。
4. 在 `Build and deployment` 中选择：
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`
5. 保存后等待 GitHub Pages 构建完成。

发布完成后，访问地址通常是：

`https://你的GitHub用户名.github.io/task-starter-prototype/`

## API 说明

页面默认使用本地识别，不需要 API。

如需使用 AI：

1. 展开“AI 配置”。
2. 选择 ChatGPT、Kimi 或 DeepSeek。
3. 填入自己的 API Key。
4. 点击“验证 API”。

验证通过后，生成报告会自动在后台使用 AI。API Key 仅保存在当前浏览器页面状态中，不会写入代码。

## 隐私说明

- 历史记录只保存在用户本机浏览器 `localStorage`。
- 静态站点本身没有后端数据库。
- 如果用户启用 AI，任务内容会发送到用户填写的 API 服务商。
