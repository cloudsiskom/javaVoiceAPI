
# Blastrequest

## Structure

`Blastrequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Callerid` | `String` | Required | - | String getCallerid() | setCallerid(String callerid) |
| `Destination` | `String` | Required | - | String getDestination() | setDestination(String destination) |
| `TextToSpeech` | `String` | Required | - | String getTextToSpeech() | setTextToSpeech(String textToSpeech) |
| `Language` | `String` | Required | - | String getLanguage() | setLanguage(String language) |
| `Gender` | `String` | Required | - | String getGender() | setGender(String gender) |
| `Repeat` | `int` | Required | - | int getRepeat() | setRepeat(int repeat) |
| `ExternalId` | `String` | Required | - | String getExternalId() | setExternalId(String externalId) |
| `CallbackUrl` | `String` | Required | - | String getCallbackUrl() | setCallbackUrl(String callbackUrl) |

## Example (as JSON)

```json
{
  "callerid": "6285757920463",
  "destination": "6285772337980",
  "text_to_speech": "Halo mas machri apa kabar? halo mas machri apa",
  "language": "id_ID",
  "gender": "FEMALE",
  "repeat": 10,
  "external_id": "[EXTERNAL_ID]",
  "callback_url": "https://eov2zjk1xwqtjan.m.pipedream.net"
}
```

