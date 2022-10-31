
# Devcie List

## Structure

`DevcieList`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Response` | `boolean` | Required | - | boolean getResponse() | setResponse(boolean response) |
| `Data` | [`List<Data1>`](../../doc/models/data-1.md) | Required | - | List<Data1> getData() | setData(List<Data1> data) |

## Example (as JSON)

```json
{
  "response": true,
  "data": [
    {
      "extension": "968976567",
      "host": "dynamic",
      "device_type": "EXTEN",
      "device_owner": "sahabat",
      "secret": "sahabat",
      "isOnline": 0,
      "device_state": "UNAVAILABLE"
    },
    {
      "extension": "961424500000013",
      "host": "192.168.1.1",
      "device_type": "TRUNK",
      "device_owner": "kiki",
      "secret": "padamunegeri",
      "isOnline": 0,
      "device_state": null
    }
  ]
}
```

