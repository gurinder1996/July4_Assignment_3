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
```

### `GET /v1/call/{call_id}`

Retrieve the status and transcript of a specific call.

### `GET /v1/agents/`

List all available agent configurations.

---

*This is a simplified overview. For a full breakdown of all parameters and models, please refer to the complete documentation within the `/docs` directory of the repository.*
```
