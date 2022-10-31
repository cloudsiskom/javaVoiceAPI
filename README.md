
# Java Voice API

## Introduction

Voice API request

## Building

Supported Java version is **8+**.

The code uses a few Maven dependencies e.g., Jackson, OkHttp,
and Apache HttpClient. The reference to these dependencies is already
added in the pom.xml file will be installed automatically. Therefore,
you will need internet access for a successful build.
 

## Test the SDK

The generated code and the server can be tested using automatically generated test cases.
JUnit is used as the testing framework and test runner.
 
## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| `httpClientConfig` | [`ReadonlyHttpClientConfiguration`](doc/http-client-configuration.md) | Http Client Configuration instance. |
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

## Authorization

This API uses `Basic Authentication`.

## List of APIs

* [Conversation AI](doc/controllers/conversation-ai.md)
* [Call](doc/controllers/call.md)
* [Masking](doc/controllers/masking.md)
* [Translation](doc/controllers/translation.md)
* [Device](doc/controllers/device.md)
* [Agent](doc/controllers/agent.md)
* [Queue](doc/controllers/queue.md)
* [Route](doc/controllers/route.md)
* [IVR](doc/controllers/ivr.md)
* [DID](doc/controllers/did.md)

## Classes Documentation

* [Utility Classes](doc/utility-classes.md)
* [HttpRequest](doc/http-request.md)
* [HttpResponse](doc/http-response.md)
* [HttpStringResponse](doc/http-string-response.md)
* [HttpContext](doc/http-context.md)
* [HttpBodyRequest](doc/http-body-request.md)
* [HttpCallback Interface](doc/http-callback-interface.md)
* [Headers](doc/headers.md)
* [ApiException](doc/api-exception.md)
* [Configuration Interface](doc/configuration-interface.md)
* [HttpClientConfiguration](doc/http-client-configuration.md)
* [HttpClientConfiguration.Builder](doc/http-client-configuration-builder.md)

