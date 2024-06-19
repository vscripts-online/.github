Hello,

Our system is built on a microservices architecture, comprising a set of services that perform specific tasks independently. The core microservices in our system include:

[Session (deprecated)](https://github.com/vscripts-online/session-ms): Manages user sessions and handles authentication processes.

[User (deprecated)](https://github.com/vscripts-online/user-ms): Manages user data and performs operations related to users.

[File](https://github.com/vscripts-online/file-ms): Stores files database, manages access, and permissions.

[Queue](https://github.com/vscripts-online/queue-ms): Processes message queues and manages asynchronous tasks.

[Consumer](https://github.com/vscripts-online/consumer) Consumers, including email senders and file uploaders, handle background tasks efficiently, ensuring optimal performance within our system

These microservices work together to form various components of our system. However, to manage direct access to these services and provide a unified interface to the outside world, we employ an [API Gateway](https://github.com/vscripts-online/api-gateway).

The API Gateway routes, authorizes, and forwards incoming requests from the outside world to the microservices. It also tracks incoming requests, applies security controls, and handles error management. This abstraction shields the complexity of our system and provides users with a single entry point.

Our API Gateway is designed to facilitate interaction with the external world while ensuring security and performance.

Current architecture:

![Architecture](https://sketchboard.me/JEqhQm2ngNq# "Architecture")
