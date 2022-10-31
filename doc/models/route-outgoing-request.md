
# Route Outgoing Request

## Structure

`RouteOutgoingRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `RouteName` | `String` | Required | - | String getRouteName() | setRouteName(String routeName) |
| `Device` | `String` | Required | - | String getDevice() | setDevice(String device) |
| `RouteTo` | `String` | Required | - | String getRouteTo() | setRouteTo(String routeTo) |
| `RouteDetail` | `String` | Required | - | String getRouteDetail() | setRouteDetail(String routeDetail) |
| `RoutePrefix` | `String` | Required | - | String getRoutePrefix() | setRoutePrefix(String routePrefix) |

## Example (as JSON)

```json
{
  "route_name": "[ROUTE_NAME]",
  "device": "[DEVICE]",
  "route_to": "[ROUTE_DESTINATION]",
  "route_detail": "[DESTINATION_DETAIL]",
  "route_prefix": "[PREFIX]"
}
```

