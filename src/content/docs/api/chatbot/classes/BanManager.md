---
editUrl: false
next: false
prev: false
title: "BanManager"
---

The ban manager of a chatroom.

## Extends

- `Base`\<`T`\>

## Type parameters

| Type parameter |
| :------ |
| `T` *extends* [`EventSubConnection`](/api/chatbot/enumerations/eventsubconnection/) |

## Constructors

### new BanManager()

```ts
new BanManager<T>(chatbot: ChatBot<T>, chatroom: ChatRoom<T>): BanManager<T>
```

Creates a new instance of the badge manager.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `chatbot` | [`ChatBot`](/api/chatbot/classes/chatbot/)\<`T`\> | The current instance of the chatbot. |
| `chatroom` | [`ChatRoom`](/api/chatbot/classes/chatroom/)\<`T`\> | The chatroom which includes this manager. |

#### Returns

[`BanManager`](/api/chatbot/classes/banmanager/)\<`T`\>

#### Overrides

`Base<T>.constructor`

#### Source

twitchfy/packages/chatbot/src/structures/managers/BanManager.ts:22

## Properties

| Property | Modifier | Type | Description | Inherited from |
| :------ | :------ | :------ | :------ | :------ |
| `chatbot` | `readonly` | [`ChatBot`](/api/chatbot/classes/chatbot/)\<`T`\> | The current instance of the chatbot. | `Base.chatbot` |
| `chatroom` | `readonly` | [`ChatRoom`](/api/chatbot/classes/chatroom/)\<`T`\> | The chatroom which includes this manager. | - |

## Methods

### add()

```ts
add(options: BanOptions): Promise<Ban<T>>
```

Ban a specific user.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `options` | [`BanOptions`](/api/chatbot/interfaces/banoptions/) | The options required for banning an user. See [BanOptions](../../api/chatbot/interfaces/banoptions). |

#### Returns

`Promise`\<[`Ban`](/api/chatbot/classes/ban/)\<`T`\>\>

A class representation of the ban. See [Ban](/api/chatbot/api/chatbot/classes/ban/).

#### Source

twitchfy/packages/chatbot/src/structures/managers/BanManager.ts:32

***

### delete()

```ts
delete(userId: string): Promise<void>
```

Deletes the ban of a specific user.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `userId` | `string` | The id of the user to unban. |

#### Returns

`Promise`\<`void`\>

#### Source

twitchfy/packages/chatbot/src/structures/managers/BanManager.ts:41
