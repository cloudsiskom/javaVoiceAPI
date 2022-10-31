# Call

```java
CallController callController = client.getCallController();
```

## Class Name

`CallController`


# Blast

SUPPORTED **LANGUAGE** :

\* id-ID  
\* en-US

**GENDER** :

\* MALE  
\* FEMALE

```java
CompletableFuture<Blast> blastAsync(
    final Blastrequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`Blastrequest`](../../doc/models/blastrequest.md) | Body, Required | - |

## Response Type

[`Blast`](../../doc/models/blast.md)

## Example Usage

```java
Blastrequest body = new Blastrequest();
body.setCallerid("6285757920463");
body.setDestination("6285772337980");
body.setTextToSpeech("Halo mas machri apa kabar? halo mas machri apa");
body.setLanguage("id_ID");
body.setGender("FEMALE");
body.setRepeat(10);
body.setExternalId("[EXTERNAL_ID]");
body.setCallbackUrl("https://eov2zjk1xwqtjan.m.pipedream.net");

callController.blastAsync(body).thenAccept(result -> {
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
  "rcode": {
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
}
```

