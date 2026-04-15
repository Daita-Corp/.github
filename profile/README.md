<div align="center">

<a href="https://daita-tech.io/"><img src="./logo.png" alt="Daita" width="300"/></a>

**AI Agent framework for data operations.**

[![X](https://img.shields.io/badge/@usedaita-000?style=flat&logo=x&logoColor=white)](https://x.com/usedaita)
[![YouTube](https://img.shields.io/badge/@usedaita-FF0000?style=flat&logo=youtube&logoColor=white)](https://www.youtube.com/@usedaita)
[![PyPI](https://img.shields.io/pypi/v/daita-agents?label=daita-agents&color=2ea44f)](https://pypi.org/project/daita-agents/)
[![PyPI](https://img.shields.io/pypi/v/daita-cli?label=daita-cli&color=2ea44f)](https://pypi.org/project/daita-cli/)
[![PyPI](https://img.shields.io/pypi/v/daita-client?label=daita-client&color=2ea44f)](https://pypi.org/project/daita-client/)

</div>

---

## What we're building

**[daita-agents](https://github.com/Daita-Corp/daita-agents)** — A Python framework for building autonomous AI agents that scale with your data. Multi provider LLM support, a rich plugin ecosystem, persistent memory, multi-agent workflows, and zero-config tracing, all with a minimal API.

```python
from daita import Agent, tool

@tool
def query_database(sql: str) -> list:
    """Run a SQL query and return results."""
    ...

agent = Agent(name="Analyst", llm_provider="openai", model="gpt-4o", tools=[query_database])
result = await agent.run("What were our top 5 products by revenue last quarter?")
```

```bash
pip install daita-agents
```

---

## Core features

- **Any LLM** — OpenAI, Anthropic, Gemini, Grok, or bring your own
- **Plugin ecosystem** — PostgreSQL, MySQL, MongoDB, Snowflake, S3, Slack, Elasticsearch, Neo4j, Chroma, Pinecone, Qdrant, and more
- **Persistent memory** — agents remember context across sessions
- **Multi-agent workflows** — connect agents into pipelines via typed relay channels
- **Automatic tracing** — tokens, latency, and cost tracked on every call
- **MCP support** — plug in any Model Context Protocol server

---

## Get started

| | |
|---|---|
| **Docs** | [docs.daita-tech.io](https://docs.daita-tech.io) |
| **PyPI** | `pip install daita-agents` |
| **Issues** | [github.com/Daita-Corp/daita-agents/issues](https://github.com/Daita-Corp/daita-agents/issues) |
| **Contact** | support@daita-tech.io |

---

_Apache 2.0 licensed. Built for developers who want agents that work in production, not just demos._
