---
editUrl: false
next: false
prev: false
title: "BasePermission"
---

Base class for building custom permissions.

## Type parameters

| Type parameter |
| :------ |
| `T` *extends* [`EventSubConnection`](/api/chatbot/enumerations/eventsubconnection/) |

## Constructors

### new BasePermission()

```ts
new BasePermission<T>(): BasePermission<T>
```

#### Returns

[`BasePermission`](/api/chatbot/classes/basepermission/)\<`T`\>

## Properties

| Property | Modifier | Type | Description |
| :------ | :------ | :------ | :------ |
| `value` | `abstract` | `string` | The value or identifier of the custom permission returned in `onPermissionsFallback`. See Command. |

## Methods

### check()

```ts
abstract check(ctx: TwitchContext<object, T>): boolean | Promise<boolean>
```

Check if the user has the custom permission to run the command.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `ctx` | [`TwitchContext`](/api/chatbot/classes/twitchcontext/)\<`object`, `T`\> | The context of the command which was run. |

#### Returns

`boolean` \| `Promise`\<`boolean`\>

If the user has the custom permission to run the command.

#### Source

twitchfy/packages/chatbot/src/structures/BasePermission.ts:15
