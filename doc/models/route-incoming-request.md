
# Route Incoming Request

## Structure

`RouteIncomingRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Did` | `String` | Required | - | String getDid() | setDid(String did) |
| `Destination` | `String` | Required | - | String getDestination() | setDestination(String destination) |
| `DestinationDetail` | `String` | Required | - | String getDestinationDetail() | setDestinationDetail(String destinationDetail) |

## Example (as JSON)

```json
{
  "did": "[DID]",
  "destination": "[DESTINATION]",
  "destination_detail": "[DESTINATION_DETAIL]"
}
```

