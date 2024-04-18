---
editUrl: false
next: false
prev: false
title: "ChannelEmote"
---

Represents a Twitch channel emote.

## Extends

- [`Emote`](/api/chatbot/classes/emote/)\<`T`, `"channel"`\>

## Type parameters

| Type parameter |
| :------ |
| `T` extends [`EventSubConnection`](/api/chatbot/enumerations/eventsubconnection/) |

## Constructors

### new ChannelEmote(chatbot, data)

```ts
new ChannelEmote<T>(chatbot: ChatBot<T>, data: ChannelEmote & Object): ChannelEmote<T>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `chatbot` | [`ChatBot`](/api/chatbot/classes/chatbot/)\<`T`\> |
| `data` | `ChannelEmote` & `Object` |

#### Returns

[`ChannelEmote`](/api/chatbot/classes/channelemote/)\<`T`\>

#### Overrides

[`Emote`](/api/chatbot/classes/emote/).[`constructor`](/api/chatbot/classes/emote/#constructors)

#### Source

[twitchapi/packages/chatbot/src/structures/ChannelEmote.ts:21](https://github.com/pablornc/twitchapi//blob/8695acad106a836c1f0fc4c57a113f17adce41f0/packages/chatbot/src/structures/ChannelEmote.ts#L21)

## Properties

| Property | Modifier | Type | Description | Inherited from |
| :------ | :------ | :------ | :------ | :------ |
| `chatbot` | `readonly` | [`ChatBot`](/api/chatbot/classes/chatbot/)\<`T`\> | The current instance of the chatbot. | [`Emote`](/api/chatbot/classes/emote/).`chatbot` |
| `emoteSetID` | `readonly` | `string` | The ID of the emote set. | - |
| `id` | `readonly` | `string` | The id of the emote. | [`Emote`](/api/chatbot/classes/emote/).`id` |
| `name` | `readonly` | `string` | The name of the emote. | [`Emote`](/api/chatbot/classes/emote/).`name` |
| `type` | `readonly` | `EmoteType` | The type of the emote. | - |

## Accessors

### animated

```ts
get animated(): boolean
```

Whether the emote is animated.

#### Returns

`boolean`

#### Source

[twitchapi/packages/chatbot/src/structures/BaseEmote.ts:62](https://github.com/pablornc/twitchapi//blob/8695acad106a836c1f0fc4c57a113f17adce41f0/packages/chatbot/src/structures/BaseEmote.ts#L62)

***

### hasDarkTheme

```ts
get hasDarkTheme(): boolean
```

Checks whether the emote is dark theme.

#### Returns

`boolean`

#### Source

[twitchapi/packages/chatbot/src/structures/Emote.ts:37](https://github.com/pablornc/twitchapi//blob/8695acad106a836c1f0fc4c57a113f17adce41f0/packages/chatbot/src/structures/Emote.ts#L37)

***

### hasLightTheme

```ts
get hasLightTheme(): boolean
```

Checks whether the emote is light theme.

#### Returns

`boolean`

#### Source

[twitchapi/packages/chatbot/src/structures/Emote.ts:30](https://github.com/pablornc/twitchapi//blob/8695acad106a836c1f0fc4c57a113f17adce41f0/packages/chatbot/src/structures/Emote.ts#L30)

***

### ownerID

```ts
get ownerID(): null | string
```

The ID of the owner of the emote.

#### Returns

`null` \| `string`

#### Source

[twitchapi/packages/chatbot/src/structures/BaseEmote.ts:41](https://github.com/pablornc/twitchapi//blob/8695acad106a836c1f0fc4c57a113f17adce41f0/packages/chatbot/src/structures/BaseEmote.ts#L41)

***

### setID

```ts
get setID(): null | string
```

The ID of the emote set.

#### Returns

`null` \| `string`

#### Source

[twitchapi/packages/chatbot/src/structures/BaseEmote.ts:48](https://github.com/pablornc/twitchapi//blob/8695acad106a836c1f0fc4c57a113f17adce41f0/packages/chatbot/src/structures/BaseEmote.ts#L48)

***

### static

```ts
get static(): boolean
```

Whether the emote is static.

#### Returns

`boolean`

#### Source

[twitchapi/packages/chatbot/src/structures/BaseEmote.ts:55](https://github.com/pablornc/twitchapi//blob/8695acad106a836c1f0fc4c57a113f17adce41f0/packages/chatbot/src/structures/BaseEmote.ts#L55)

***

### tier

```ts
get tier(): null | number
```

Returns the subscription tier necessary to use the emote. If the emote is not a subscription emote, it will return null.

#### Returns

`null` \| `number`

#### Source

[twitchapi/packages/chatbot/src/structures/ChannelEmote.ts:38](https://github.com/pablornc/twitchapi//blob/8695acad106a836c1f0fc4c57a113f17adce41f0/packages/chatbot/src/structures/ChannelEmote.ts#L38)

## Methods

### fetch()

```ts
fetch(): Promise<null | ChannelEmote<T>>
```

Fetches the emote from the API.

#### Returns

`Promise`\<`null` \| [`ChannelEmote`](/api/chatbot/classes/channelemote/)\<`T`\>\>

The fetched emote. Returns null if the emote was not found.

#### Inherited from

[`Emote`](/api/chatbot/classes/emote/).[`fetch`](/api/chatbot/classes/emote/#fetch)

#### Source

[twitchapi/packages/chatbot/src/structures/BaseEmote.ts:86](https://github.com/pablornc/twitchapi//blob/8695acad106a836c1f0fc4c57a113f17adce41f0/packages/chatbot/src/structures/BaseEmote.ts#L86)

***

### getURL()

```ts
getURL(options?: EmoteURLOptions): string
```

Gets the URL of the emote.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `options`? | [`EmoteURLOptions`](/api/chatbot/interfaces/emoteurloptions/) | The options to get the URL of the emote. |

#### Returns

`string`

Returns the URL of the emote.

#### Inherited from

[`Emote`](/api/chatbot/classes/emote/).[`getURL`](/api/chatbot/classes/emote/#geturl)

#### Source

[twitchapi/packages/chatbot/src/structures/Emote.ts:46](https://github.com/pablornc/twitchapi//blob/8695acad106a836c1f0fc4c57a113f17adce41f0/packages/chatbot/src/structures/Emote.ts#L46)

***

### isChannel()

```ts
isChannel(): this is ChannelEmote<T>
```

Overrides isChannel method from BaseEmote to assert this as ChannelEmote and not BaseEmote.

#### Returns

`this is ChannelEmote<T>`

Whether the emote is a channel emote.

#### Overrides

[`Emote`](/api/chatbot/classes/emote/).[`isChannel`](/api/chatbot/classes/emote/#ischannel)

#### Source

[twitchapi/packages/chatbot/src/structures/ChannelEmote.ts:31](https://github.com/pablornc/twitchapi//blob/8695acad106a836c1f0fc4c57a113f17adce41f0/packages/chatbot/src/structures/ChannelEmote.ts#L31)

***

### isGlobal()

```ts
isGlobal(): this is BaseEmote<T, "global">
```

Check if the emote is a global Twitch emote.

#### Returns

`this is BaseEmote<T, "global">`

A boolean indicating whether the emote is a global Twitch emote.

#### Inherited from

[`Emote`](/api/chatbot/classes/emote/).[`isGlobal`](/api/chatbot/classes/emote/#isglobal)

#### Source

[twitchapi/packages/chatbot/src/structures/BaseEmote.ts:70](https://github.com/pablornc/twitchapi//blob/8695acad106a836c1f0fc4c57a113f17adce41f0/packages/chatbot/src/structures/BaseEmote.ts#L70)