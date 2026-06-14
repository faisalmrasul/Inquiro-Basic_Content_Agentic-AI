# Setup Guide – Advanced AI Agent v2

## 1. Prerequisites

- n8n instance (self-hosted recommended)
- Accounts for:
  - Groq API
  - Supabase
  - SerpAPI
  - Gmail (for OAuth2)

## 2. Import Workflow

1. Open n8n
2. Go to **Workflows** → **Import from File**
3. Upload `workflow.json`

## 3. Configure Credentials

### Groq API
- Create credential named `Groq account`
- Paste your Groq API key

### Supabase
- Create two HTTP Request credentials or use Header Auth
- Base URL: `https://oevhfludpmfykcogniuf.supabase.co`
- API Key: (from your Supabase project)

### Gmail
- Use OAuth2 credential

### SerpAPI
- Add your SerpAPI key in the Web Search node

## 4. Environment Variables (Optional)

Copy `.env.example` → `.env` and fill in values.

## 5. Test the Workflow

Use the pinned data (NASA Mars article) or send a POST request to the webhook:

```json
{
  "userMessage": "Summarize this article and give latest updates",
  "userContent": "Paste article text here..."
}