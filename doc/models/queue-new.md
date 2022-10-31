
# Queue New

## Structure

`QueueNew`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Response` | `boolean` | Required | - | boolean getResponse() | setResponse(boolean response) |
| `Data` | [`Data5`](../../doc/models/data-5.md) | Required | - | Data5 getData() | setData(Data5 data) |

## Example (as JSON)

```json
{
  "response": true,
  "data": {
    "queue_name": "queue-151-3",
    "ring_strategy": "ringall"
  }
}
```

