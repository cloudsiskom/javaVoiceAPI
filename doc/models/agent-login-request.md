
# Agent Login Request

## Structure

`AgentLoginRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `ActionType` | `String` | Required | - | String getActionType() | setActionType(String actionType) |
| `AgentCode` | `String` | Required | - | String getAgentCode() | setAgentCode(String agentCode) |
| `Extension` | `String` | Required | - | String getExtension() | setExtension(String extension) |
| `AgentPassword` | `String` | Required | - | String getAgentPassword() | setAgentPassword(String agentPassword) |

## Example (as JSON)

```json
{
  "action_type": "[ACTION]",
  "agent_code": "[AGENT_CODE]",
  "extension": "[EXTENSION TO LOGIN]",
  "agent_password": "[AGENT_PASSWORD]"
}
```

