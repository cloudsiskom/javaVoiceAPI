
# Translation Delete Exception

## Structure

`TranslationDeleteException`

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
  "error_code": 1402,
  "reason": "transaction id : 64c7a1e218b004054e49d304814cd1b0 Not found"
}
```

