
# Device

## Structure

`Device`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Response` | `boolean` | Required | - | boolean getResponse() | setResponse(boolean response) |
| `Data` | [`Data`](../../doc/models/data.md) | Required | - | Data getData() | setData(Data data) |

## Example (as JSON)

```json
{
  "response": true,
  "data": {
    "extension": "961424500000013",
    "secret": "padamunegeri",
    "device_owner": "kiki"
  }
}
```

