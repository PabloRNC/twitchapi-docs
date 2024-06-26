---
editUrl: false
next: false
prev: false
title: "BaseUserWithoutUsername"
---

The base class for a user without an username.

## Extends

- `Base`\<`T`\>

## Type parameters

| Type parameter |
| :------ |
| `T` *extends* [`EventSubConnection`](/api/chatbot/enumerations/eventsubconnection/) |

## Constructors

### new BaseUserWithoutUsername()

```ts
new BaseUserWithoutUsername<T>(chatbot: ChatBot<T>, data: Omit<BaseUserData, "login">): BaseUserWithoutUsername<T>
```

Creates a new instance of the base user without an username.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `chatbot` | [`ChatBot`](/api/chatbot/classes/chatbot/)\<`T`\> | The current instance of the chatbot. |
| `data` | `Omit`\<[`BaseUserData`](/api/chatbot/interfaces/baseuserdata/), `"login"`\> | The base data of the user. |

#### Returns

[`BaseUserWithoutUsername`](/api/chatbot/classes/baseuserwithoutusername/)\<`T`\>

#### Overrides

`Base<T>.constructor`

#### Source

twitchfy/packages/chatbot/src/structures/BaseUserWithoutUsername.ts:28

## Properties

| Property | Modifier | Type | Description | Inherited from |
| :------ | :------ | :------ | :------ | :------ |
| `chatbot` | `readonly` | [`ChatBot`](/api/chatbot/classes/chatbot/)\<`T`\> | The current instance of the chatbot. | `Base.chatbot` |
| `dislayName` | `readonly` | `string` | The display name of the user. | - |
| `id` | `readonly` | `string` | The id of the user. | - |

## Methods

### fetch()

```ts
fetch(): Promise<User<T>>
```

Fetches the current user from the API.

#### Returns

`Promise`\<[`User`](/api/chatbot/classes/user/)\<`T`\>\>

The fetched user from the API.

#### Source

twitchfy/packages/chatbot/src/structures/BaseUserWithoutUsername.ts:38

***

### inStream()

```ts
inStream(): Promise<boolean>
```

Returns whether the user is currently in stream or not.

#### Returns

`Promise`\<`boolean`\>

A boolean indicating whether the user is currently streaming.

#### Source

twitchfy/packages/chatbot/src/structures/BaseUserWithoutUsername.ts:64

***

### stream()

```ts
stream(): Promise<null | Stream<T>>
```

Fetches the current stream of the user from the API.

#### Returns

`Promise`\<`null` \| [`Stream`](/api/chatbot/classes/stream/)\<`T`\>\>

The current stream or null if the stream is offline.

#### Source

twitchfy/packages/chatbot/src/structures/BaseUserWithoutUsername.ts:53

***

### toString()

```ts
toString(): string
```

Returns the mention of the user.

#### Returns

`string`

#### Source

twitchfy/packages/chatbot/src/structures/BaseUserWithoutUsername.ts:45

***

### whisper()

```ts
whisper(message: string): Promise<void>
```

Sends a whisper to the user.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `message` | `string` | The message to send. |

#### Returns

`Promise`\<`void`\>

#### Source

twitchfy/packages/chatbot/src/structures/BaseUserWithoutUsername.ts:74
