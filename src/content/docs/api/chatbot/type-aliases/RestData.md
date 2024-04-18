---
editUrl: false
next: false
prev: false
title: "RestData"
---

```ts
type RestData<T, K>: Object;
```

The rest of data which builds up the [MessageData](../../api/chatbot/type-aliases/messagedata).

## Type parameters

| Type parameter | Value |
| :------ | :------ |
| `T` extends [`EventSubConnection`](/api/chatbot/enumerations/eventsubconnection/) | - |
| `K` extends [`OptionsRecord`](/api/chatbot/type-aliases/optionsrecord/) | `Object` |

## Type declaration

| Member | Type |
| :------ | :------ |
| `commandName` | `string` |
| `options` | [`CommandOptionsAux`](/api/chatbot/type-aliases/commandoptionsaux/)\<`T`, `K`\> |
| `prefix` | `string` |

## Source

[twitchapi/packages/chatbot/src/types/MessageData.ts:23](https://github.com/pablornc/twitchapi//blob/8695acad106a836c1f0fc4c57a113f17adce41f0/packages/chatbot/src/types/MessageData.ts#L23)