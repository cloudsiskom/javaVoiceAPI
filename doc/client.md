
# Client Class Documentation

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| `httpClientConfig` | [`ReadonlyHttpClientConfiguration`](http-client-configuration.md) | Http Client Configuration instance. |
| `username` | `String` |  |
| `password` | `String` |  |

The API client can be initialized as follows:

```java
SiskomVoiceAPIClient client = new SiskomVoiceAPIClient.Builder()
    .httpClientConfig(configBuilder -> configBuilder
            .timeout(0))
    .basicAuthCredentials("username", "password")
    .environment(Environment.PRODUCTION)
    .build();
```

## siskom Voice APIClient Class

The gateway for the SDK. This class acts as a factory for the Controllers and also holds the configuration of the SDK.

### Controllers

| Name | Description | Return Type |
|  --- | --- | --- |
| `getCallController()` | Provides access to Call controller. | `CallController` |
| `getMaskingController()` | Provides access to Masking controller. | `MaskingController` |
| `getTranslationController()` | Provides access to Translation controller. | `TranslationController` |
| `getDeviceController()` | Provides access to Device controller. | `DeviceController` |
| `getAgentController()` | Provides access to Agent controller. | `AgentController` |
| `getQueueController()` | Provides access to Queue controller. | `QueueController` |
| `getRouteController()` | Provides access to Route controller. | `RouteController` |
| `getIVRController()` | Provides access to IVR controller. | `IVRController` |
| `getConversationAIController()` | Provides access to ConversationAI controller. | `ConversationAIController` |
| `getDIDController()` | Provides access to DID controller. | `DIDController` |

### Methods

| Name | Description | Return Type |
|  --- | --- | --- |
| `shutdown()` | Shutdown the underlying HttpClient instance. | `void` |
| `getEnvironment()` | Current API environment. | `Environment` |
| `getHttpClient()` | The HTTP Client instance to use for making HTTP requests. | `HttpClient` |
| `getHttpClientConfig()` | Http Client Configuration instance. | [`ReadonlyHttpClientConfiguration`](http-client-configuration.md) |
| `getBaseUri(Server server)` | Get base URI by current environment | `String` |
| `getBaseUri()` | Get base URI by current environment | `String` |

