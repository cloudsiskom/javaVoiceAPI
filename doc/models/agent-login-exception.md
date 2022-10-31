
# Agent Login Exception

## Structure

`AgentLoginException`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Response` | `boolean` | Required | - | boolean getResponse() | setResponse(boolean response) |
| `ErrorCode` | `int` | Required | - | int getErrorCode() | setErrorCode(int errorCode) |
| `Reason` | `String` | Required | - | String getReason() | setReason(String reason) |

## Example (as JSON)

```json
{
  "response": false,
  "error_code": 1409,
  "reason": "Extension not found"
}
```

