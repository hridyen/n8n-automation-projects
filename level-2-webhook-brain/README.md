# Level 2 – Webhook Validation System (n8n)

## Problem
APIs and forms should not blindly trust incoming data.

## Solution
This workflow implements a webhook-based validation system that:
- Accepts incoming JSON data
- Normalizes and validates input
- Returns proper HTTP responses (200 / 400)

## Flow
- Webhook trigger
- Input normalization
- Validation using JavaScript
- IF logic for trust boundary
- Proper API response via Respond to Webhook

## Concepts Used
- Webhooks
- Backend-style validation
- Trust boundaries
- HTTP status codes
- API response design

## Testing
Example curl request:
```bash
curl -X POST http://localhost:5678/webhook-test/lead-intake \
-H "Content-Type: application/json" \
-d '{"name":"Hriday","email":"hriday@gmail.com","phone":"9876543210"}'
