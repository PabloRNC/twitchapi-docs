---
editUrl: false
next: false
prev: false
title: "BaseCheermote"
---

Represents a base cheermote returned by the EventSub.

## Extends

- `Base`\<`T`\>

## Type parameters

| Type parameter |
| :------ |
| `T` *extends* [`EventSubConnection`](/api/chatbot/enumerations/eventsubconnection/) |

## Constructors

### new BaseCheermote()

```ts
new BaseCheermote<T>(chatbot: ChatBot<T>, data: Cheermote & object): BaseCheermote<T>
```

Creates a new instance of the base cheermote.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `chatbot` | [`ChatBot`](/api/chatbot/classes/chatbot/)\<`T`\> | The current instance of the chatbot. |
| `data` | `Cheermote` & `object` | The data of the cheermote returned by the EventSub. |

#### Returns

[`BaseCheermote`](/api/chatbot/classes/basecheermote/)\<`T`\>

#### Overrides

`Base<T>.constructor`

#### Source

twitchfy/packages/chatbot/src/structures/BaseCheermote.ts:37

## Properties

| Property | Modifier | Type | Description | Inherited from |
| :------ | :------ | :------ | :------ | :------ |
| `bits` | `readonly` | `number` | The bits that were cheered with the cheermote. | - |
| `chatbot` | `readonly` | [`ChatBot`](/api/chatbot/classes/chatbot/)\<`T`\> | The current instance of the chatbot. | `Base.chatbot` |
| `prefix` | `readonly` | `string` | The prefix of the cheermote. | - |
| `tier` | `readonly` | `number` | The tier level of the cheermote. | - |

## Accessors

### content

```ts
get content(): string
```

The content of the cheermote. This is the prefix followed by the bits cheered.

#### Returns

`string`

#### Source

twitchfy/packages/chatbot/src/structures/BaseCheermote.ts:48

## Methods

### fetch()

```ts
fetch(): Promise<null | Cheermote<T>>
```

Fetches the cheermote from the API returning the information of it.

#### Returns

`Promise`\<`null` \| [`Cheermote`](/api/chatbot/classes/cheermote/)\<`T`\>\>

The cheermote if it exists. If not it will return `null` (basically this is 99.99% impossible).

#### Source

twitchfy/packages/chatbot/src/structures/BaseCheermote.ts:56
