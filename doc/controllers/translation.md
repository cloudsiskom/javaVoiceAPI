# Translation

```java
TranslationController translationController = client.getTranslationController();
```

## Class Name

`TranslationController`

## Methods

* [Translation Delete](../../doc/controllers/translation.md#translation-delete)
* [Translation Setup](../../doc/controllers/translation.md#translation-setup)


# Translation Delete

```java
CompletableFuture<Void> translationDeleteAsync(
    final TranslationDeleteRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`TranslationDeleteRequest`](../../doc/models/translation-delete-request.md) | Body, Required | - |

## Response Type

`void`

## Example Usage

```java
TranslationDeleteRequest body = new TranslationDeleteRequest();
body.setTransactionId("[TRANSACTION_ID]");

translationController.translationDeleteAsync(body).thenAccept(result -> {
    // TODO success callback handler
}).exceptionally(exception -> {
    // TODO failure callback handler
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 404 | Not Found | [`TranslationDeleteException`](../../doc/models/translation-delete-exception.md) |


# Translation Setup

```java
CompletableFuture<TranslationSetup> translationSetupAsync(
    final TranslationSetupRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`TranslationSetupRequest`](../../doc/models/translation-setup-request.md) | Body, Required | - |

## Response Type

[`TranslationSetup`](../../doc/models/translation-setup.md)

## Example Usage

```java
TranslationSetupRequest body = new TranslationSetupRequest();
body.setFromNumber("[FROM_NUMBER]");
body.setCallerDidgateway("[DID_GATEWAY]");
body.setCalledDidgateway("[DID_GATEWAY]");
body.setDestinationNumber("[DESTINATION]");
body.setExternalId("[EXTERNAL_ID]");

translationController.translationSetupAsync(body).thenAccept(result -> {
    // TODO success callback handler
}).exceptionally(exception -> {
    // TODO failure callback handler
    return null;
});
```

## Example Response *(as JSON)*

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

