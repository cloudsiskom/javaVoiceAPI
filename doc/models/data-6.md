
# Data 6

## Structure

`Data6`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `QueueId` | `int` | Required | - | int getQueueId() | setQueueId(int queueId) |
| `QueueName` | `String` | Required | - | String getQueueName() | setQueueName(String queueName) |
| `Musiclass` | `String` | Required | - | String getMusiclass() | setMusiclass(String musiclass) |
| `Strategy` | `String` | Required | - | String getStrategy() | setStrategy(String strategy) |
| `Members` | [`List<Member>`]($m/Data6Members) | Required | - | List<Member> getMembers() | setMembers(List<Member> members) |

## Example (as JSON)

```json
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
}
```

