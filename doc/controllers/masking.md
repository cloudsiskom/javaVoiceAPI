# Masking

masking api lets you to use your original phone number as callerid at our SIP trunk

```java
MaskingController maskingController = client.getMaskingController();
```

## Class Name

`MaskingController`

## Methods

* [Request](../../doc/controllers/masking.md#request)
* [Delete](../../doc/controllers/masking.md#delete)
* [List](../../doc/controllers/masking.md#list)


# Request

```java
CompletableFuture<Request> requestAsync(
    final Requestrequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`Requestrequest`](../../doc/models/requestrequest.md) | Body, Required | - |

## Response Type

[`Request`](../../doc/models/request.md)

## Example Usage

```java
Requestrequest body = new Requestrequest();
body.setCallerId("[CALLER_ID]");

maskingController.requestAsync(body).thenAccept(result -> {
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
  "caller_id": "628198788686",
  "isActive": 0
}
```


# Delete

```java
CompletableFuture<Delete> deleteAsync(
    final Deleterequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`Deleterequest`](../../doc/models/deleterequest.md) | Body, Required | - |

## Response Type

[`Delete`](../../doc/models/delete.md)

## Example Usage

```java
Deleterequest body = new Deleterequest();
body.setCallerId("[CALLER_ID]");

maskingController.deleteAsync(body).thenAccept(result -> {
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
  "caller_id": "628198788686",
  "action": "delete"
}
```


# List

```java
CompletableFuture<List> listAsync()
```

## Response Type

[`List`](../../doc/models/list.md)

## Example Usage

```java
maskingController.listAsync().thenAccept(result -> {
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
  "data": []
}
```

