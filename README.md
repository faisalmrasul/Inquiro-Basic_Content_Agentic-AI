# Advanced AI Agent v2

A sophisticated **agentic AI workflow** built with n8n featuring memory, tool use, intelligent routing, self-critique, and professional email delivery.

## ✨ Features

- **Persistent Memory** via Supabase (user profile + conversation history)
- **Agentic Planning & Intelligent Routing** using LLM
- **Tool Use** – Web search with SerpAPI (conditional)
- **Self-Critique System** (Critic Agent with scoring & improvement suggestions)
- **Professional HTML Email Delivery** with quality badges and metadata
- **Robust Session & Request Management**
- **Error Handling & Partial Retry Logic**

## 🎯 Primary Use Cases

- Summarizing articles, PDFs, and reports
- Researching current events or topics
- Providing deep analysis and insights
- Automated client or team reporting
- Personal knowledge assistant

## 🛠 Tech Stack

- **Orchestration**: n8n
- **LLM**: Groq (Llama-3.3-70b-versatile)
- **Memory Store**: Supabase
- **Web Search**: SerpAPI
- **Email**: Gmail (OAuth2)
- **Trigger**: Webhook

## Quick Start

1. Import `workflow.json` into your n8n instance
2. Configure credentials (Groq, Supabase, Gmail, SerpAPI)
3. Activate the workflow
4. Call the webhook with `userMessage` (and optional `userContent`)

See [setup-guide.md](setup-guide.md) for detailed instructions.

## Repository Contents

- `workflow.json` – Complete n8n workflow
- `setup-guide.md` – Setup instructions
- `improvements.md` – Future roadmap
- `.env.example` – Environment variables template

## License

MIT License – see [LICENSE](LICENSE) file.
