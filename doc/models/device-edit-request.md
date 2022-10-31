
# Device Edit Request

## Structure

`DeviceEditRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `Extension` | `String` | Required | - | String getExtension() | setExtension(String extension) |
| `DeviceOwner` | `String` | Required | - | String getDeviceOwner() | setDeviceOwner(String deviceOwner) |
| `Secret` | `String` | Required | - | String getSecret() | setSecret(String secret) |

## Example (as JSON)

```json
{
  "extension": "[DEVICE_EXTENSION]",
  "device_owner": "[DEVICE_OWNER]",
  "secret": "[DEVICE_SECRET]"
}
```

