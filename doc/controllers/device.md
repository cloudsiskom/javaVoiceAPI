# Device

```java
DeviceController deviceController = client.getDeviceController();
```

## Class Name

`DeviceController`

## Methods

* [Device](../../doc/controllers/device.md#device)
* [Devcie List](../../doc/controllers/device.md#devcie-list)
* [Device Edit](../../doc/controllers/device.md#device-edit)
* [Device Delete](../../doc/controllers/device.md#device-delete)


# Device

DEVICE_TYPE :

\*   TRUNK (This will be sip trunk with dedicated IP Address)
\*   EXTEN (Extension)

```java
CompletableFuture<Device> deviceAsync(
    final DeviceRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`DeviceRequest`](../../doc/models/device-request.md) | Body, Required | - |

## Response Type

[`Device`](../../doc/models/device.md)

## Example Usage

```java
DeviceRequest body = new DeviceRequest();
body.setDeviceType("[DEVICE_TYPE]");
body.setDeviceOwner("[DEVICE_OWNER]");
body.setExtension("[DEVICE_NAME / EXTENSION]");
body.setSecret("[DEVICE_SECRET]");
body.setIpAddress("[DEVICE_IP_ADDRESS]");

deviceController.deviceAsync(body).thenAccept(result -> {
    // TODO success callback handler
}).exceptionally(exception -> {
    // TODO failure callback handler
    return null;
});
```

## Example Response *(as JSON)*

```json
{
  "response": true,
  "data": {
    "extension": "961424500000013",
    "secret": "padamunegeri",
    "device_owner": "kiki"
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 403 | Forbidden | [`Device1Exception`](../../doc/models/device-1-exception.md) |


# Devcie List

```java
CompletableFuture<DevcieList> devcieListAsync()
```

## Response Type

[`DevcieList`](../../doc/models/devcie-list.md)

## Example Usage

```java
deviceController.devcieListAsync().thenAccept(result -> {
    // TODO success callback handler
}).exceptionally(exception -> {
    // TODO failure callback handler
    return null;
});
```

## Example Response *(as JSON)*

```json
{
  "response": true,
  "data": [
    {
      "extension": "968976567",
      "host": "dynamic",
      "device_type": "EXTEN",
      "device_owner": "sahabat",
      "secret": "sahabat",
      "isOnline": 0,
      "device_state": "UNAVAILABLE"
    },
    {
      "extension": "961424500000013",
      "host": "192.168.1.1",
      "device_type": "TRUNK",
      "device_owner": "kiki",
      "secret": "padamunegeri",
      "isOnline": 0,
      "device_state": null
    }
  ]
}
```


# Device Edit

```java
CompletableFuture<Void> deviceEditAsync(
    final DeviceEditRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`DeviceEditRequest`](../../doc/models/device-edit-request.md) | Body, Required | - |

## Response Type

`void`

## Example Usage

```java
DeviceEditRequest body = new DeviceEditRequest();
body.setExtension("[DEVICE_EXTENSION]");
body.setDeviceOwner("[DEVICE_OWNER]");
body.setSecret("[DEVICE_SECRET]");

deviceController.deviceEditAsync(body).thenAccept(result -> {
    // TODO success callback handler
}).exceptionally(exception -> {
    // TODO failure callback handler
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 403 | Forbidden | [`DeviceEditException`](../../doc/models/device-edit-exception.md) |


# Device Delete

```java
CompletableFuture<Void> deviceDeleteAsync(
    final DeviceDeleteRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`DeviceDeleteRequest`](../../doc/models/device-delete-request.md) | Body, Required | - |

## Response Type

`void`

## Example Usage

```java
DeviceDeleteRequest body = new DeviceDeleteRequest();
body.setExtension("[DEVICE_EXTENSION / NAME]");

deviceController.deviceDeleteAsync(body).thenAccept(result -> {
    // TODO success callback handler
}).exceptionally(exception -> {
    // TODO failure callback handler
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 404 | Not Found | [`DeviceDeleteException`](../../doc/models/device-delete-exception.md) |

