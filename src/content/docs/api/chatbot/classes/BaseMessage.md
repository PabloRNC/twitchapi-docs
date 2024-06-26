---
editUrl: false
next: false
prev: false
title: "BaseMessage"
---

The base class for a message.

## Extends

- `Base`\<`T`\>

## Extended by

- [`Message`](/api/chatbot/classes/message/)
- [`MessageReplyParent`](/api/chatbot/classes/messagereplyparent/)
- [`MessageReplyThread`](/api/chatbot/classes/messagereplythread/)

## Type parameters

| Type parameter |
| :------ |
| `T` *extends* [`EventSubConnection`](/api/chatbot/enumerations/eventsubconnection/) |

## Constructors

### new BaseMessage()

```ts
new BaseMessage<T>(chatbot: ChatBot<T>, data: BaseMessageData): BaseMessage<T>
```

Creates a new instance of the base message.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `chatbot` | [`ChatBot`](/api/chatbot/classes/chatbot/)\<`T`\> | The current instance of the chatbot. |
| `data` | [`BaseMessageData`](/api/chatbot/interfaces/basemessagedata/) | The base data of the message. |

#### Returns

[`BaseMessage`](/api/chatbot/classes/basemessage/)\<`T`\>

#### Overrides

`Base<T>.constructor`

#### Source

twitchfy/packages/chatbot/src/structures/BaseMessage.ts:36

## Properties

| Property | Modifier | Type | Description | Inherited from |
| :------ | :------ | :------ | :------ | :------ |
| `author` | `readonly` | [`BaseUser`](/api/chatbot/classes/baseuser/)\<`T`\> | The author of the message. | - |
| `chatbot` | `readonly` | [`ChatBot`](/api/chatbot/classes/chatbot/)\<`T`\> | The current instance of the chatbot. | `Base.chatbot` |
| `content` | `readonly` | `null` \| `string` | The content of the message. | - |
| `id` | `readonly` | `string` | The id of the message. | - |

## Accessors

### chatroomId

```ts
get chatroomId(): string
```

The Id of the chatroom where the message was sent.

#### Returns

`string`

#### Source

twitchfy/packages/chatbot/src/structures/BaseMessage.ts:64

***

### self

```ts
get self(): boolean
```

Whether the message was sent by the chatbot.

#### Returns

`boolean`

#### Source

twitchfy/packages/chatbot/src/structures/BaseMessage.ts:71

## Methods

### delete()

```ts
delete(): Promise<void>
```

Deletes the message from the chatroom.

#### Returns

`Promise`\<`void`\>

#### Source

twitchfy/packages/chatbot/src/structures/BaseMessage.ts:48

***

### reply()

```ts
reply(message: string): Promise<BaseMessage<T>>
```

Replies to the message.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | The message to reply with. |

#### Returns

`Promise`\<[`BaseMessage`](/api/chatbot/classes/basemessage/)\<`T`\>\>

The message that was sent as a reply.

#### Source

twitchfy/packages/chatbot/src/structures/BaseMessage.ts:57
