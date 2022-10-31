
# Queue New Request

## Structure

`QueueNewRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `QueueName` | `String` | Required | - | String getQueueName() | setQueueName(String queueName) |
| `RingStrategy` | `String` | Required | - | String getRingStrategy() | setRingStrategy(String ringStrategy) |

## Example (as JSON)

```json
{
  "queue_name": "[QUEUE_NAME]",
  "ring_strategy": "[RING_STRATEGY]"
}
```

