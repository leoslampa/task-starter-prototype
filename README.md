# 一句话任务问法助手

[English](#task-question-helper)

一个面向项目负责人的静态网页工具，用于拆解一句话任务，并生成更好开口的关键问法。

核心输出：

- 任务拆解：梳理初步边界、交付方向、关键里程碑和风险。
- 优先问法：生成不超过 5 个关键问题，并给出更容易被回答的问法。
- 轻量提醒：提示用户记得保留必要沟通记录。

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

1. 点击页面中的“启用 AI”。
2. 阅读并同意《使用说明与隐私声明》。
3. 填入本机账号名称。
4. 选择 ChatGPT、Kimi 或 DeepSeek。
5. 填入自己的 API Key。
6. 点击“验证 API”。

验证通过后，生成报告会自动在后台使用 AI。

## 隐私说明

- 本应用采用本机账号模式，不需要注册，也不提供云端账号。
- 用户输入的账号名仅用于在当前浏览器中区分本机配置。
- 历史记录只保存在用户本机浏览器 `localStorage`。
- 静态站点本身没有后端数据库。
- 内容、配置、使用记录和 API Key 仅保存在当前浏览器中。
- 本应用不会收集、保存、分析或追踪任何使用行为、输入内容、生成结果或 API Key。
- 如果用户启用 AI，任务内容会发送到用户填写的 API 服务商。
- API Key 由用户自己提供，模型费用由用户的模型服务商账户承担。
- 请勿在公共设备上保存 API Key。

## 版权声明

本应用及其界面、功能设计、提示词模板和相关代码版权归作者所有。未经许可，不得复制、修改、分发、商用或二次发布。

用户通过自有 API Key 调用模型生成的内容，由用户自行负责保存、使用和确认权利归属。

---

# Task Question Helper

[中文](#一句话任务问法助手)

Task Question Helper is a static web tool for project owners who receive vague or one-sentence assignments. It breaks down the task and generates clearer, easier-to-ask questions.

Core outputs:

- Task breakdown: clarify initial boundaries, deliverable direction, milestones, and risks.
- Suggested questions: generate up to 5 key questions with wording that is easier to answer.
- Light reminder: remind users to keep necessary communication records.

## Local Use

Open `index.html` directly in a browser to try it locally.

## Public Deployment

This is a pure frontend static site. It can be deployed to:

- Vercel
- Netlify
- Cloudflare Pages
- GitHub Pages

Deploying the current directory is enough.

### GitHub Pages

1. Create a public GitHub repository, for example `task-starter-prototype`.
2. Push the local code to the `main` branch.
3. Open `Settings` -> `Pages` in the repository.
4. Under `Build and deployment`, choose:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`
5. Save and wait for GitHub Pages to finish building.

The public URL is usually:

`https://your-github-username.github.io/task-starter-prototype/`

## API

The app uses local recognition by default and does not require an API.

To enable AI:

1. Click `Enable AI`.
2. Read and agree to the Usage and Privacy Notice.
3. Enter a local account name.
4. Choose ChatGPT, Kimi, or DeepSeek.
5. Enter your own API key.
6. Click `Verify API`.

After verification, report generation will use AI in the background.

## Privacy

- The app uses a local account mode. It does not require registration or provide cloud accounts.
- The account name is only used to distinguish local configurations in the current browser.
- History is stored only in the user’s browser `localStorage`.
- The static site itself has no backend database.
- Content, configuration, usage records, and API keys are stored only in the current browser.
- The app does not collect, store, analyze, or track usage behavior, input content, generated results, or API keys.
- If AI is enabled, task content will be sent to the model provider configured by the user.
- API keys are provided by users themselves, and model usage fees are charged by their own model service accounts.
- Do not save API keys on public devices.

## Copyright

The application, including its interface, functional design, prompt templates, and related code, is copyrighted by the author. Copying, modifying, distributing, commercial use, or republication without permission is not allowed.

Content generated through a user’s own API key is the user’s responsibility to save, use, and confirm rights ownership.
