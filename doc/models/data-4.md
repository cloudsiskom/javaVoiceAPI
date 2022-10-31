
# Data 4

## Structure

`Data4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `int` | Required | - | int getId() | setId(int id) |
| `CustomerCode` | `String` | Required | - | String getCustomerCode() | setCustomerCode(String customerCode) |
| `AgentCode` | `int` | Required | - | int getAgentCode() | setAgentCode(int agentCode) |
| `AgentName` | `String` | Required | - | String getAgentName() | setAgentName(String agentName) |
| `RequirePassword` | `int` | Required | - | int getRequirePassword() | setRequirePassword(int requirePassword) |
| `AgentPassword` | `int` | Required | - | int getAgentPassword() | setAgentPassword(int agentPassword) |
| `Lastlogin` | `int` | Required | - | int getLastlogin() | setLastlogin(int lastlogin) |
| `IsActive` | `int` | Required | - | int getIsActive() | setIsActive(int isActive) |
| `IsLogin` | `int` | Required | - | int getIsLogin() | setIsLogin(int isLogin) |
| `LoginChannel` | `String` | Required | - | String getLoginChannel() | setLoginChannel(String loginChannel) |
| `LoginExtension` | `String` | Required | - | String getLoginExtension() | setLoginExtension(String loginExtension) |
| `LoginUniqueid` | `String` | Required | - | String getLoginUniqueid() | setLoginUniqueid(String loginUniqueid) |

## Example (as JSON)

```json
{
  "id": 34,
  "customer_code": "GOJEK",
  "agent_code": 9610002,
  "agent_name": "queue-152",
  "require_password": 1,
  "agent_password": 4321,
  "lastlogin": 0,
  "isActive": 1,
  "isLogin": 0,
  "login_channel": null,
  "login_extension": null,
  "login_uniqueid": null
}
```

