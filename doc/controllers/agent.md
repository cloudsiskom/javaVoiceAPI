# Agent

```java
AgentController agentController = client.getAgentController();
```

## Class Name

`AgentController`

## Methods

* [Agent New](../../doc/controllers/agent.md#agent-new)
* [Agent Delete](../../doc/controllers/agent.md#agent-delete)
* [Agent List](../../doc/controllers/agent.md#agent-list)
* [Agent Login](../../doc/controllers/agent.md#agent-login)


# Agent New

ACTION :

\*   new (New agent)
\*   edit (Edit existing Agent)

```java
CompletableFuture<AgentNew> agentNewAsync(
    final AgentNewRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`AgentNewRequest`](../../doc/models/agent-new-request.md) | Body, Required | - |

## Response Type

[`AgentNew`](../../doc/models/agent-new.md)

## Example Usage

```java
AgentNewRequest body = new AgentNewRequest();
body.setAction("[ACTION]");
body.setAgentCode("[AGENT_CODE]");
body.setAgentName("[AGENT_NAME]");
body.setAgentPassword("[AGENT_PASSWORD]");

agentController.agentNewAsync(body).thenAccept(result -> {
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
    "action": "new",
    "agent_code": "10002",
    "agent_name": "queue-152",
    "agent_password": "4321"
  }
}
```


# Agent Delete

```java
CompletableFuture<AgentDelete> agentDeleteAsync(
    final AgentDeleteRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`AgentDeleteRequest`](../../doc/models/agent-delete-request.md) | Body, Required | - |

## Response Type

[`AgentDelete`](../../doc/models/agent-delete.md)

## Example Usage

```java
AgentDeleteRequest body = new AgentDeleteRequest();
body.setAgentCode("[AGENT_CODE]");

agentController.agentDeleteAsync(body).thenAccept(result -> {
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
    "agent_code": "10002"
  }
}
```


# Agent List

```java
CompletableFuture<AgentList> agentListAsync()
```

## Response Type

[`AgentList`](../../doc/models/agent-list.md)

## Example Usage

```java
agentController.agentListAsync().thenAccept(result -> {
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
      "id": 34,
      "customer_code": "GOJEK",
      "agent_code": 9610002,
      "agent_name": "queue-152",
      "require_password": 1,
      "agent_password": 4321,
      "lastlogin": 0,
      "isActive": 1,
      "isLogin": 0,
      "login_channel": null,
      "login_extension": null,
      "login_uniqueid": null
    }
  ]
}
```


# Agent Login

**ACTION** :

\*   login (Login agent to EXTENSION)
\*   logoff (logoff agent from EXTENSION)

```java
CompletableFuture<Void> agentLoginAsync(
    final AgentLoginRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`AgentLoginRequest`](../../doc/models/agent-login-request.md) | Body, Required | - |

## Response Type

`void`

## Example Usage

```java
AgentLoginRequest body = new AgentLoginRequest();
body.setActionType("[ACTION]");
body.setAgentCode("[AGENT_CODE]");
body.setExtension("[EXTENSION TO LOGIN]");
body.setAgentPassword("[AGENT_PASSWORD]");

agentController.agentLoginAsync(body).thenAccept(result -> {
    // TODO success callback handler
}).exceptionally(exception -> {
    // TODO failure callback handler
    return null;
});
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 403 | Forbidden | [`AgentLoginException`](../../doc/models/agent-login-exception.md) |

