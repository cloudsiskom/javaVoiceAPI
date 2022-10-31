
# Device Request

## Structure

`DeviceRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `DeviceType` | `String` | Required | - | String getDeviceType() | setDeviceType(String deviceType) |
| `DeviceOwner` | `String` | Required | - | String getDeviceOwner() | setDeviceOwner(String deviceOwner) |
| `Extension` | `String` | Required | - | String getExtension() | setExtension(String extension) |
| `Secret` | `String` | Required | - | String getSecret() | setSecret(String secret) |
| `IpAddress` | `String` | Required | - | String getIpAddress() | setIpAddress(String ipAddress) |

## Example (as JSON)

```json
{
  "device_type": "[DEVICE_TYPE]",
  "device_owner": "[DEVICE_OWNER]",
  "extension": "[DEVICE_NAME / EXTENSION]",
  "secret": "[DEVICE_SECRET]",
  "ip_address": "[DEVICE_IP_ADDRESS]"
}
```

