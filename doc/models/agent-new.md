
# Agent New

## Structure

`AgentNew`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Response` | `boolean` | Required | - | boolean getResponse() | setResponse(boolean response) |
| `Data` | [`Data2`](../../doc/models/data-2.md) | Required | - | Data2 getData() | setData(Data2 data) |

## Example (as JSON)

```json
{
  "response": true,
  "data": {
    "action": "new",
    "agent_code": "10002",
    "agent_name": "queue-152",
    "agent_password": "4321"
  }
}
```

