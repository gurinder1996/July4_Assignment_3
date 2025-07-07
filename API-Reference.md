# API Reference: The Core Endpoints

Here's a high-level overview of the primary API endpoints you'll use to control your agents.

### `POST /v1/call/`

This is the main endpoint to initiate an outbound call.

**Request Body:**
```json
{
  "phone_number": "+15551234567",
  "agent_id": "sales-agent-001",
  "assistant_config": {
    "model": "gpt-4o",
    "prompt": "You are a helpful sales assistant for AeroGlide Motors..."
  },
  "metadata": {
    "lead_id": "xyz-987"
  }
}
