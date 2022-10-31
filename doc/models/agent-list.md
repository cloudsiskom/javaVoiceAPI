
# Agent List

## Structure

`AgentList`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Response` | `boolean` | Required | - | boolean getResponse() | setResponse(boolean response) |
| `Data` | [`List<Data4>`](../../doc/models/data-4.md) | Required | - | List<Data4> getData() | setData(List<Data4> data) |

## Example (as JSON)

```json
{
  "response": true,
  "data": [
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
  ]
}
```

