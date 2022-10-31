
# Outgoing Route

## Structure

`OutgoingRoute`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `int` | Required | - | int getId() | setId(int id) |
| `CustomerCode` | `String` | Required | - | String getCustomerCode() | setCustomerCode(String customerCode) |
| `Extension` | `String` | Required | - | String getExtension() | setExtension(String extension) |
| `RouteTo` | `String` | Required | - | String getRouteTo() | setRouteTo(String routeTo) |
| `RouteDetail` | `String` | Required | - | String getRouteDetail() | setRouteDetail(String routeDetail) |
| `TechPrefix` | `String` | Required | - | String getTechPrefix() | setTechPrefix(String techPrefix) |
| `CreateDate` | `String` | Required | - | String getCreateDate() | setCreateDate(String createDate) |
| `IsActive` | `int` | Required | - | int getIsActive() | setIsActive(int isActive) |

## Example (as JSON)

```json
{
  "id": 582,
  "customer_code": "GOJEK",
  "extension": "ALL",
  "route_to": "PROVIDER",
  "route_detail": "6285592055236",
  "tech_prefix": "",
  "create_date": "2022-09-14T19:40:24.000Z",
  "isActive": 1
}
```

