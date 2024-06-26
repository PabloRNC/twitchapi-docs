---
editUrl: false
next: false
prev: false
title: "ChannelFollow"
---

Represents a channel follow event.

## Extends

- `Base`\<`T`\>

## Type parameters

| Type parameter |
| :------ |
| `T` *extends* [`EventSubConnection`](/api/chatbot/enumerations/eventsubconnection/) |

## Constructors

### new ChannelFollow()

```ts
new ChannelFollow<T>(chatbot: ChatBot<T>, data: ChannelFollowMessage<EventSubConnectionMap[T]>): ChannelFollow<T>
```

Creates a new instance of the channel follow event.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `chatbot` | [`ChatBot`](/api/chatbot/classes/chatbot/)\<`T`\> | The current instance of the chatbot. |
| `data` | `ChannelFollowMessage`\<`EventSubConnectionMap`\[`T`\]\> | The data of the follow event returned from the EventSub. |

#### Returns

[`ChannelFollow`](/api/chatbot/classes/channelfollow/)\<`T`\>

#### Overrides

`Base<T>.constructor`

#### Source

twitchfy/packages/chatbot/src/structures/ChannelFollow.ts:38

## Properties

| Property | Modifier | Type | Description | Inherited from |
| :------ | :------ | :------ | :------ | :------ |
| `broadcaster` | `readonly` | [`BaseUser`](/api/chatbot/classes/baseuser/)\<`T`\> | The broadcaster of the channel who was followed. | - |
| `chatbot` | `readonly` | [`ChatBot`](/api/chatbot/classes/chatbot/)\<`T`\> | The current instance of the chatbot. | `Base.chatbot` |
| `followedAt` | `readonly` | `Date` | The date when the follower followed the channel. | - |
| `follower` | `readonly` | [`BaseUser`](/api/chatbot/classes/baseuser/)\<`T`\> | The follower who followed the channel. | - |

## Accessors

### broadcasterId

```ts
get broadcasterId(): string
```

The Id of the broadcaster who was followed.

#### Returns

`string`

#### Source

twitchfy/packages/chatbot/src/structures/ChannelFollow.ts:49

***

### chatroomId

```ts
get chatroomId(): string
```

The Id of the chatroom where the follow event occurred.

#### Returns

`string`

#### Source

twitchfy/packages/chatbot/src/structures/ChannelFollow.ts:63

***

### followerId

```ts
get followerId(): string
```

The Id of the follower who followed the channel.

#### Returns

`string`

#### Source

twitchfy/packages/chatbot/src/structures/ChannelFollow.ts:56
