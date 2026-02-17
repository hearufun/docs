# Contributing to TalkOS Documentation

Thank you for your interest in improving TalkOS documentation! We welcome contributions from the community.

## Documentation Structure

| Directory | Content |
|-----------|----------|
| `/` | Core pages (introduction, quickstart, concepts) |
| `/guides` | Integration guides (Plivo, Exotel, webhooks) |
| `/api-reference` | API endpoint documentation |
| `/api-reference/features` | Feature-specific APIs |

## How to Contribute

### Quick Edits (GitHub)

1. Navigate to the page you want to edit
2. Click the pencil icon ("Edit this file")
3. Make your changes
4. Submit a pull request with a clear description

### Local Development

```bash
# Clone the repository
git clone https://github.com/hearufun/docs.git
cd docs

# Install CLI
npm i -g mint

# Preview locally
mint dev
```

View at `http://localhost:3000`

## Writing Guidelines

### Voice & Tone
- **Active voice**: "Run the command" not "The command should be run"
- **Direct address**: Use "you" instead of "the user"
- **Concise**: One idea per sentence
- **Goal-first**: Start with what the user wants to accomplish

### API Documentation
- Include cURL, Node.js, and Python examples
- Document all request/response fields
- Add error response examples
- Use realistic sample data

### Code Examples
```bash
# Good: Specific, copyable
curl -X POST https://api.talkos.io/api/calls/start \
  -H "x-api-key: your_api_key" \
  -H "x-tenant-id: tenant_123"

# Avoid: Vague placeholders
curl -X POST <url> -H <headers>
```

## TalkOS Terminology

| Use | Instead of |
|-----|------------|
| tenant | organization, account |
| call session | call instance |
| knowledge base | document store |
| webhook | callback URL |

## Need Help?

Email: docs@talkos.io
