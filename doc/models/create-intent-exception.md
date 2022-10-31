
# Create Intent Exception

## Structure

`CreateIntentException`

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
  "error_code": 1406,
  "reason": "Intent save error, please try again, possible reason : display name exist !"
}
```

