# MyTracker S2S API Overview

MyTracker, a Russian analytics service, provides a server-to-server (S2S) API that allows users to send data to the MyTracker server. This API is designed to facilitate the upload of various events, such as user authorizations, payments, deliveries, and more. The uploaded events are then incorporated into the project data and displayed in the MyTracker reports.

## Accessing the S2S API
To access the S2S API, users need to follow these steps:

1. Register in MyTracker.
2. Obtain an authentication key known as the S2S API key.

To simplify the integration process, MyTracker offers an open-source PHP Software Development Kit (SDK). This SDK provides a set of libraries and tools that make it easier to work with the MyTracker S2S API in PHP.

## PHP SDK and Examples
The PHP SDK provided by MyTracker offers a convenient starting point for developers looking to integrate their applications with MyTracker. It includes the `Example` class, which demonstrates the usage of various API features. Let's take a look at some examples:

### Checking S2S API Accessibility
The `Example` class provides a method called `getActualVersion()` that allows developers to check if the S2S API is accessible without any credentials. It retrieves and displays the current version of the API.

### Checking Account Token
To ensure proper authentication, developers can use the `testAppAccess()` method provided by the `Example` class. This method requires an application ID (`$yourAppId`) and an account token (`$yourAccountToken`). It verifies the access to the MyTracker application associated with the provided credentials and returns a response code.

### Sending Events
The `Example` class demonstrates how to send different types of events using the MyTracker S2S API. Developers can utilize the following methods:

- `sendRegistrationEvent($yourAppId, $yourAccountToken)`: Sends a registration event to MyTracker.
- `sendLoginEvent($yourAppId, $yourAccountToken)`: Sends a login event to MyTracker.
- `sendCustomEvent($yourAppId, $yourAccountToken)`: Sends a custom event to MyTracker.
- `sendCustomRevenue($yourAppId, $yourAccountToken)`: Sends a custom revenue event to MyTracker.

By calling these methods and providing the appropriate application ID and account token, developers can integrate event tracking seamlessly into their PHP applications.

## Conclusion
PHP plays a crucial role in the integration of MyTracker's S2S API. The PHP SDK provided by MyTracker simplifies the process of sending data and events to the MyTracker server, allowing developers to leverage the analytics capabilities of the MyTracker service effectively in their PHP applications.
