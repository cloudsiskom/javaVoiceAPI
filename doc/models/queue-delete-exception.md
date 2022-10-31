
# Queue Delete Exception

## Structure

`QueueDeleteException`

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
  "error_code": 1403,
  "reason": "Queue not found"
}
```

