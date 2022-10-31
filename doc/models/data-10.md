
# Data 10

## Structure

`Data10`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `CustomerCode` | `String` | Required | - | String getCustomerCode() | setCustomerCode(String customerCode) |
| `Id` | `int` | Required | - | int getId() | setId(int id) |
| `Active` | `int` | Required | - | int getActive() | setActive(int active) |
| `Did` | `String` | Required | - | String getDid() | setDid(String did) |
| `DidType` | `String` | Required | - | String getDidType() | setDidType(String didType) |
| `ActivationCost` | `int` | Required | - | int getActivationCost() | setActivationCost(int activationCost) |
| `Incoming` | `String` | Required | - | String getIncoming() | setIncoming(String incoming) |
| `DestinationDetail` | `String` | Required | - | String getDestinationDetail() | setDestinationDetail(String destinationDetail) |
| `IsActive` | [`Data10IsActive`]($m/Data10IsActive) | Required | - | Data10IsActive getIsActive() | setIsActive(Data10IsActive isActive) |

## Example (as JSON)

```json
{
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
```

