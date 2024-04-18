---
editUrl: false
next: false
prev: false
title: "MentionOption"
---

Represents a mention option.

## Type parameters

| Type parameter | Value |
| :------ | :------ |
| `T` extends `null` | `null` |
| `K` extends `boolean` | `false` |

## Constructors

### new MentionOption(options)

```ts
new MentionOption<T, K>(options?: Object): MentionOption<T, K>
```

Creates a new instance of the mention option.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `options`? | `Object` | The options of the mention option. |
| `options.grouped`? | `K` | - |

#### Returns

[`MentionOption`](/api/chatbot/classes/mentionoption/)\<`T`, `K`\>

#### Source

[twitchapi/packages/chatbot/src/structures/MentionOption.ts:25](https://github.com/pablornc/twitchapi//blob/8695acad106a836c1f0fc4c57a113f17adce41f0/packages/chatbot/src/structures/MentionOption.ts#L25)

## Properties

| Property | Modifier | Type | Description |
| :------ | :------ | :------ | :------ |
| `defaultValue` | `readonly` | `T` | The default value of the mention option. Always null as actually there is not planned way to set a default value. |
| `grouped` | `readonly` | `K` | Whether the mention option is grouped into more than two types of mention. |
| `type` | `readonly` | `"mention"` | The type of the mention option. It's always mention. |