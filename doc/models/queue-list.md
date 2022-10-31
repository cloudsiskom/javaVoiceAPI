
# Queue List

## Structure

`QueueList`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Response` | `boolean` | Required | - | boolean getResponse() | setResponse(boolean response) |
| `Data` | [`List<Data6>`](../../doc/models/data-6.md) | Required | - | List<Data6> getData() | setData(List<Data6> data) |

## Example (as JSON)

```json
{
  "response": true,
  "data": [
    {
      "queue_id": 35,
      "queue_name": "96789665",
      "musiclass": "default",
      "strategy": "ringall",
      "members": [
        {
          "member": "SIP/968976567"
        }
      ]
    },
    {
      "queue_id": 36,
      "queue_name": "96queue-151-3",
      "musiclass": "default",
      "strategy": "ringall",
      "members": []
    }
  ]
}
```

