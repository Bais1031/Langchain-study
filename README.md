# LangChain 学习笔记

本仓库用于系统学习 [LangChain](https://www.langchain.com/)（Python），从基础调用到链式编排、工具与智能体、RAG 等主题逐步深入。

## 环境要求

- Python **3.10+**（与 `pyproject.toml` 一致）
- 建议使用 [uv](https://github.com/astral-sh/uv) 或 `pip` 管理依赖

### 安装依赖

根据你要跟的教程版本，安装对应包。常见组合：

```bash
# 使用 uv（推荐）
uv sync
# 若尚未在 pyproject 中声明依赖，可先手动安装：
uv add langchain langchain-core langchain-community

# 若使用 OpenAI（或其它厂商），再添加对应集成包，例如：
uv add langchain-openai
```

调用大模型需要配置 **API Key**（如 `OPENAI_API_KEY`），请使用环境变量或 `.env`，**不要将密钥提交到 Git**。

## 官方与社区资源

| 资源 | 说明 |
|------|------|
| [LangChain Python 文档](https://python.langchain.com/) | 概念说明、API、教程 |
| [LangChain GitHub](https://github.com/langchain-ai/langchain) | 源码与 Issue |
| [LangSmith](https://smith.langchain.com/) | 可选：追踪与调试链路与 Agent |

文档站点会随版本更新，遇到与本地代码不一致时，以你安装的包版本对应的文档为准。

