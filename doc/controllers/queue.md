# Queue

```java
QueueController queueController = client.getQueueController();
```

## Class Name

`QueueController`

## Methods

* [Queue New](../../doc/controllers/queue.md#queue-new)
* [Queue Delete](../../doc/controllers/queue.md#queue-delete)
* [Queue List](../../doc/controllers/queue.md#queue-list)
* [Queue Add Agent](../../doc/controllers/queue.md#queue-add-agent)
* [Queue Remove Agent](../../doc/controllers/queue.md#queue-remove-agent)


# Queue New

RING_STRATEGY :

\*   ringall: ring all available channels until one answers (default)
\*   roundrobin: take turns ringing each available interface (deprecated in 1.4, use rrmemory)
\*   leastrecent: ring interface which was least recently called by this queue
\*   fewestcalls: ring the one with fewest completed calls from this queue
\*   random: ring random interface
\*   rrmemory: round robin with memory, remember where we left off last ring pass

```java
CompletableFuture<QueueNew> queueNewAsync(
    final QueueNewRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`QueueNewRequest`](../../doc/models/queue-new-request.md) | Body, Required | - |

## Response Type

[`QueueNew`](../../doc/models/queue-new.md)

## Example Usage

```java
QueueNewRequest body = new QueueNewRequest();
body.setQueueName("[QUEUE_NAME]");
body.setRingStrategy("[RING_STRATEGY]");

queueController.queueNewAsync(body).thenAccept(result -> {
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
    "queue_name": "queue-151-3",
    "ring_strategy": "ringall"
  }
}
```


# Queue Delete

```java
CompletableFuture<Void> queueDeleteAsync(
    final QueueDeleteRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`QueueDeleteRequest`](../../doc/models/queue-delete-request.md) | Body, Required | - |

## Response Type

`void`

## Example Usage

```java
QueueDeleteRequest body = new QueueDeleteRequest();
body.setQueueName("[QUEUE_NAME]");

queueController.queueDeleteAsync(body).thenAccept(result -> {
    // TODO success callback handler
}).exceptionally(exception -> {
    // TODO failure callback handler
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 404 | Not Found | [`QueueDeleteException`](../../doc/models/queue-delete-exception.md) |


# Queue List

```java
CompletableFuture<QueueList> queueListAsync()
```

## Response Type

[`QueueList`](../../doc/models/queue-list.md)

## Example Usage

```java
queueController.queueListAsync().thenAccept(result -> {
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
      "queue_id": 35,
      "queue_name": "96789665",
      "musiclass": "default",
      "strategy": "ringall",
      "members": [
        {
          "member": "SIP/968976567"
        }
      ]
    },
    {
      "queue_id": 36,
      "queue_name": "96queue-151-3",
      "musiclass": "default",
      "strategy": "ringall",
      "members": []
    }
  ]
}
```


# Queue Add Agent

**AGENT_TYPE** :

\*   SIP (Agent is SIP device / Extension)
\*   local (Agent is AGENT_CODE)

```java
CompletableFuture<Void> queueAddAgentAsync(
    final QueueAddAgentRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`QueueAddAgentRequest`](../../doc/models/queue-add-agent-request.md) | Body, Required | - |

## Response Type

`void`

## Example Usage

```java
QueueAddAgentRequest body = new QueueAddAgentRequest();
body.setQueueName("[QUEUE_NAME]");
body.setAgents("[AGENT]");
body.setAgentType("[AGENT_TYPE]");

queueController.queueAddAgentAsync(body).thenAccept(result -> {
    // TODO success callback handler
}).exceptionally(exception -> {
    // TODO failure callback handler
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 404 | Not Found | [`QueueAddAgentException`](../../doc/models/queue-add-agent-exception.md) |


# Queue Remove Agent

**AGENT_TYPE** :

\* SIP (Agent is SIP device / Extension)  
\* local (Agent is AGENT_CODE)

```java
CompletableFuture<Void> queueRemoveAgentAsync(
    final QueueRemoveAgentRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`QueueRemoveAgentRequest`](../../doc/models/queue-remove-agent-request.md) | Body, Required | - |

## Response Type

`void`

## Example Usage

```java
QueueRemoveAgentRequest body = new QueueRemoveAgentRequest();
body.setQueueName("[QUEUE_NAME]");
body.setAgents("[agent]");
body.setAgentType("[AGENT_TYPE]");

queueController.queueRemoveAgentAsync(body).thenAccept(result -> {
    // TODO success callback handler
}).exceptionally(exception -> {
    // TODO failure callback handler
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 404 | Not Found | [`QueueRemoveAgentException`](../../doc/models/queue-remove-agent-exception.md) |

