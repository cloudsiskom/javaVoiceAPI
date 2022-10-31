
# Translation Setup

## Structure

`TranslationSetup`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Respose` | `boolean` | Required | - | boolean getRespose() | setRespose(boolean respose) |
| `Action` | `String` | Required | - | String getAction() | setAction(String action) |
| `TransactionId` | `String` | Required | - | String getTransactionId() | setTransactionId(String transactionId) |
| `ExternalId` | `String` | Required | - | String getExternalId() | setExternalId(String externalId) |
| `FromNumber` | `String` | Required | - | String getFromNumber() | setFromNumber(String fromNumber) |
| `DestinationNumber` | `String` | Required | - | String getDestinationNumber() | setDestinationNumber(String destinationNumber) |
| `CallerDidgateway` | `String` | Required | - | String getCallerDidgateway() | setCallerDidgateway(String callerDidgateway) |
| `CalledDidgateway` | `String` | Required | - | String getCalledDidgateway() | setCalledDidgateway(String calledDidgateway) |

## Example (as JSON)

```json
{
  "respose": true,
  "action": "setup",
  "transaction_id": "cf54bfa60c738515574809998f71bd62",
  "external_id": "1000",
  "from_number": "62811949736",
  "destination_number": "6285161422932",
  "caller_didgateway": "6285757920463",
  "called_didgateway": "6285757920463"
}
```

