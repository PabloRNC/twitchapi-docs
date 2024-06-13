---
editUrl: false
next: false
prev: false
title: "WebhookShardStart"
---

Message emitted when a shard is starting with a webhook transport.

## Properties

| Property | Type |
| :------ | :------ |
| `shard` | `object` |
| `shard.id` | `string` |
| `shard.status` | `string` |
| `shard.transport` | `object` |
| `shard.transport.callback` | `string` |
| `shard.transport.method` | `"webhook"` |
| `shard.transport.secret` | `string` |
| `topic` | `"shard.webhook.start"` |