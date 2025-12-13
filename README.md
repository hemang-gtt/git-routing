https://claude.ai/share/f7f0d196-43a4-4d63-9bb8-80272d60d4d8


https://claude.ai/share/7ad838a9-c31e-4f85-a87c-0186de62b010




pending service architecture


https://claude.ai/share/7ad838a9-c31e-4f85-a87c-0186de62b010

Pending orchestrator



├── server.js                # Only starts HTTP server
├── app.js                   # Express app config
│
├── bootstrap/
│   └── index.js             # Starts all consumers & schedulers
│
├── consumers/
│   ├── streamConsumer.js
│   ├── resolvePendingConsumer.js
│   └── index.js
│
├── schedulers/
│   └── pendingRetryScheduler.js
│
├── services/
│   ├── apiService.js
│   └── pendingHandler.js
│
├── locks/
│   └── semaphore.js
│
├── models/
│   └── *.model.js
│
├── utils/
│   ├── redis.js
│   ├── mongo.js
│   └── commonUtils.js
│
├── errors/
│   ├── anakatechErrorHandler.js
│   └── softSwissErrorHandler.js
│
└config/
  ── index.js
