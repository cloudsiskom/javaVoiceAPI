
# Data 1

## Structure

`Data1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Extension` | `String` | Required | - | String getExtension() | setExtension(String extension) |
| `Host` | `String` | Required | - | String getHost() | setHost(String host) |
| `DeviceType` | `String` | Required | - | String getDeviceType() | setDeviceType(String deviceType) |
| `DeviceOwner` | `String` | Required | - | String getDeviceOwner() | setDeviceOwner(String deviceOwner) |
| `Secret` | `String` | Required | - | String getSecret() | setSecret(String secret) |
| `IsOnline` | `int` | Required | - | int getIsOnline() | setIsOnline(int isOnline) |
| `DeviceState` | `String` | Required | - | String getDeviceState() | setDeviceState(String deviceState) |

## Example (as JSON)

```json
{
  "extension": "968976567",
  "host": "dynamic",
  "device_type": "EXTEN",
  "device_owner": "sahabat",
  "secret": "sahabat",
  "isOnline": 0,
  "device_state": "UNAVAILABLE"
}
```

