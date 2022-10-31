
# Route Outgoing

## Structure

`RouteOutgoing`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Response` | `boolean` | Required | - | boolean getResponse() | setResponse(boolean response) |
| `Device` | `String` | Required | - | String getDevice() | setDevice(String device) |
| `RouteTo` | `String` | Required | - | String getRouteTo() | setRouteTo(String routeTo) |
| `RouteDetail` | `String` | Required | - | String getRouteDetail() | setRouteDetail(String routeDetail) |

## Example (as JSON)

```json
{
  "response": true,
  "device": "8210000000001",
  "route_to": "RANDOM",
  "route_detail": "RDM1"
}
```

