
# Incoming Route

## Structure

`IncomingRoute`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Id` | `int` | Required | - | int getId() | setId(int id) |
| `TransactionId` | `String` | Required | - | String getTransactionId() | setTransactionId(String transactionId) |
| `CustomerCode` | `String` | Required | - | String getCustomerCode() | setCustomerCode(String customerCode) |
| `Did` | `String` | Required | - | String getDid() | setDid(String did) |
| `Destination` | `String` | Required | - | String getDestination() | setDestination(String destination) |
| `DestinationDetail` | `String` | Required | - | String getDestinationDetail() | setDestinationDetail(String destinationDetail) |
| `CreateDate` | `String` | Required | - | String getCreateDate() | setCreateDate(String createDate) |
| `IsActive` | `int` | Required | - | int getIsActive() | setIsActive(int isActive) |

## Example (as JSON)

```json
{
  "id": 57,
  "transaction_id": null,
  "customer_code": "GOJEK",
  "did": "6285757920462",
  "destination": "DTMFTEST",
  "destination_detail": null,
  "create_date": "2022-08-23T22:57:32.000Z",
  "isActive": 1
}
```

