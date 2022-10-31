
# Rcode

## Structure

`Rcode`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `TransactionId` | `String` | Required | - | String getTransactionId() | setTransactionId(String transactionId) |
| `CallbackKey` | `String` | Required | - | String getCallbackKey() | setCallbackKey(String callbackKey) |
| `Destination` | `String` | Required | - | String getDestination() | setDestination(String destination) |
| `TextToSpeech` | `String` | Required | - | String getTextToSpeech() | setTextToSpeech(String textToSpeech) |
| `Language` | `String` | Required | - | String getLanguage() | setLanguage(String language) |
| `Gender` | `String` | Required | - | String getGender() | setGender(String gender) |
| `VoiceRepeat` | `String` | Required | - | String getVoiceRepeat() | setVoiceRepeat(String voiceRepeat) |
| `ExternalId` | `String` | Required | - | String getExternalId() | setExternalId(String externalId) |
| `CallbackUrl` | `String` | Required | - | String getCallbackUrl() | setCallbackUrl(String callbackUrl) |

## Example (as JSON)

```json
{
  "transaction_id": "489EF4175D9E35DDAEFD74839DB9558D",
  "callback_key": "25c1e6ec24db6cf8bcff665761e1c985",
  "destination": "62127867676",
  "text_to_speech": "Hai.... Selamat datang saudara-saudaraku, anda adalah pelanggan utama hari ini, selamat yaaa gaeees!",
  "language": "id-ID",
  "gender": "FEMALE",
  "VoiceRepeat": "2",
  "external_id": "93894893483984938",
  "callback_url": "http"
}
```

