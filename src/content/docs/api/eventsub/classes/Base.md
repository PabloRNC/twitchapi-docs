---
editUrl: false
next: false
prev: false
title: "Base"
---

The base class for all the structures.

## Extended by

- [`ChannelUpdateCategory`](/api/eventsub/classes/channelupdatecategory/)
- [`BaseStream`](/api/eventsub/classes/basestream/)
- [`BaseUser`](/api/eventsub/classes/baseuser/)
- [`BaseMessage`](/api/eventsub/classes/basemessage/)
- [`BaseSubscriptionMessage`](/api/eventsub/classes/basesubscriptionmessage/)

## Type parameters

| Type parameter | Value |
| :------ | :------ |
| `T` *extends* [`SubscriptionTypes`](/api/eventsub/enumerations/subscriptiontypes/) | - |
| `K` *extends* [`ConnectionTypes`](/api/eventsub/type-aliases/connectiontypes/) | [`ConnectionTypes`](/api/eventsub/type-aliases/connectiontypes/) |

## Constructors

### new Base()

```ts
new Base<T, K>(connection: K, subscription: SubscriptionType<T, K>): Base<T, K>
```

Builds up a Base message.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `connection` | `K` | The EventSub connection used. |
| `subscription` | [`SubscriptionType`](/api/eventsub/type-aliases/subscriptiontype/)\<`T`, `K`\> | The subscription which trigger this message. |

#### Returns

[`Base`](/api/eventsub/classes/base/)\<`T`, `K`\>

#### Source

twitchfy/packages/eventsub/src/structures/messages/Base.ts:26

## Properties

| Property | Modifier | Type | Description |
| :------ | :------ | :------ | :------ |
| `connection` | `readonly` | `K` | The EventSub connection used. |
| `subscription` | `readonly` | [`SubscriptionType`](/api/eventsub/type-aliases/subscriptiontype/)\<`T`, `K`\> | The subscription which trigger this message. |
