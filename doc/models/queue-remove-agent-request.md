
# Queue Remove Agent Request

## Structure

`QueueRemoveAgentRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `QueueName` | `String` | Required | - | String getQueueName() | setQueueName(String queueName) |
| `Agents` | `String` | Required | - | String getAgents() | setAgents(String agents) |
| `AgentType` | `String` | Required | - | String getAgentType() | setAgentType(String agentType) |

## Example (as JSON)

```json
{
  "queue_name": "[QUEUE_NAME]",
  "agents": "[agent]",
  "agent_type": "[AGENT_TYPE]"
}
```

