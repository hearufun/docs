# TalkOS Documentation - AI Agent Instructions

## About TalkOS

TalkOS is a **multi-tenant AI Voice Calling API** platform. The documentation covers:

- Voice calling APIs (Plivo, Exotel providers)
- Real-time AI conversation with GPT-4/Claude
- Call analytics, transcription, sentiment analysis
- Knowledge base (RAG), voice biometrics, compliance

## Project Structure

```
/                    # Core pages (introduction, quickstart, auth)
/guides/             # Integration guides (plivo, exotel, webhooks)
/api-reference/      # API endpoints
  /tenant/           # Tenant management
  /calls/            # Call operations  
  /inbound/          # Inbound calling
  /numbers/          # Phone number management
  /analytics/        # Analytics APIs
  /features/         # Advanced features (masking, tags, etc.)
```

## Terminology

| Term | Meaning |
|------|----------|
| Tenant | Customer account with isolated data |
| callUuid | Unique call identifier |
| Bot number | AI-enabled inbound phone number |
| Tool calling | AI executing functions during calls |
| Knowledge Base | RAG document store for AI context |

## API Conventions

- Base URL: `https://api.talkos.io`
- Auth: `x-api-key` + `x-tenant-id` headers
- Response format: JSON
- Errors: Standard HTTP codes with `error` object

## Writing Standards

- Active voice, second person ("you")
- Include cURL, Node.js, Python examples
- Document all request/response fields
- Add realistic sample values
- Use proper MDX components (CodeGroup, ParamField, Note, Warning)

## Commands

```bash
mint dev          # Local preview
mint broken-links # Check links
```
