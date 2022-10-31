
# Translation Setup Request

## Structure

`TranslationSetupRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `FromNumber` | `String` | Required | - | String getFromNumber() | setFromNumber(String fromNumber) |
| `CallerDidgateway` | `String` | Required | - | String getCallerDidgateway() | setCallerDidgateway(String callerDidgateway) |
| `CalledDidgateway` | `String` | Required | - | String getCalledDidgateway() | setCalledDidgateway(String calledDidgateway) |
| `DestinationNumber` | `String` | Required | - | String getDestinationNumber() | setDestinationNumber(String destinationNumber) |
| `ExternalId` | `String` | Required | - | String getExternalId() | setExternalId(String externalId) |

## Example (as JSON)

```json
{
  "from_number": "[FROM_NUMBER]",
  "caller_didgateway": "[DID_GATEWAY]",
  "called_didgateway": "[DID_GATEWAY]",
  "destination_number": "[DESTINATION]",
  "external_id": "[EXTERNAL_ID]"
}
```

