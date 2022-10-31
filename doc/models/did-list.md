
# DID List

## Structure

`DIDList`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Response` | `boolean` | Required | - | boolean getResponse() | setResponse(boolean response) |
| `Data` | [`List<Data10>`](../../doc/models/data-10.md) | Required | - | List<Data10> getData() | setData(List<Data10> data) |

## Example (as JSON)

```json
{
  "response": null,
  "data": {
    "customer_code": "GOJEK",
    "id": 2,
    "active": 1,
    "did": "6285757920463",
    "did_type": "MVN",
    "activation_cost": 100000,
    "incoming": "TRUNK",
    "destination_detail": "CVAI",
    "isActive": 1
  }
}
```

