
# WeChat Channel Schema

```
https://ns.adobe.com/xdm/channels/wechat
```

WeChat Platform Notification channel.

| [Abstract](../../abstract.md) | [Extensible](../../extensions.md) | [Status](../../status.md) | [Identifiable](../../id.md) | [Custom Properties](../../extensions.md) | [Additional Properties](../../extensions.md) | Defined In |
|-------------------------------|-----------------------------------|---------------------------|-----------------------------|------------------------------------------|----------------------------------------------|------------|
| Can be instantiated | Yes | Experimental | No | Forbidden | Permitted | [channels/wechat.schema.json](channels/wechat.schema.json) |
## Schema Hierarchy

* WeChat Channel `https://ns.adobe.com/xdm/channels/wechat`
  * [Extensibility Base Schema](../common/extensible.schema.md) `https://ns.adobe.com/xdm/common/extensible`
  * [Experience Channel](channel.schema.md) `https://ns.adobe.com/xdm/channels/channel`


## WeChat Channel Example
```json
{
  "@id": "https://ns.adobe.com/xdm/channels/wechat",
  "@type": "https://ns.adobe.com/xdm/channel-types/messaging"
}
```

# WeChat Channel Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [@id](#id) | `const` | **Required** | WeChat Channel (this schema) |
| [@type](#type) | `const` | Optional | WeChat Channel (this schema) |
| [xdm:contentTypes](#xdmcontenttypes) | `const` | Optional | WeChat Channel (this schema) |
| [xdm:locationTypes](#xdmlocationtypes) | `const` | Optional | WeChat Channel (this schema) |
| [xdm:mediaAction](#xdmmediaaction) | `string` | Optional | [Experience Channel](channel.schema.md#xdmmediaaction) |
| [xdm:mediaType](#xdmmediatype) | `string` | Optional | [Experience Channel](channel.schema.md#xdmmediatype) |
| [xdm:metricTypes](#xdmmetrictypes) | `const` | Optional | WeChat Channel (this schema) |
| [xdm:mode](#xdmmode) | `const` | Optional | WeChat Channel (this schema) |
| [xdm:nameAtSource](#xdmnameatsource) | `string` | Optional | [Experience Channel](channel.schema.md#xdmnameatsource) |
| `*` | any | Additional | this schema *allows* additional properties |

## @id

The ID uniquely identifies the channel. Each specific experience channel defines a constant `@id`.

`@id`
* is **required**
* type: `const`
* defined in this schema

The value of this property **must** be equal to:

```json
"https://ns.adobe.com/xdm/channels/wechat"
```





## @type

The `@type` property is used to provide a rough classification of channels with similar properties.

`@type`
* is optional
* type: `const`
* defined in this schema

The value of this property **must** be equal to:

```json
"https://ns.adobe.com/xdm/channel-types/messaging"
```


### @type Known Values
| Value | Description |
|-------|-------------|
| `https://ns.adobe.com/xdm/channel-types/web` | The world wide web, including mobile web |
| `https://ns.adobe.com/xdm/channel-types/social` | Social media platforms |
| `https://ns.adobe.com/xdm/channel-types/mobile` | Mobile applications |
| `https://ns.adobe.com/xdm/channel-types/messaging` | Instant Messaging |
| `https://ns.adobe.com/xdm/channel-types/email` | E-Mail |
| `https://ns.adobe.com/xdm/channel-types/offline` | Non-Digital experience channels |




## xdm:contentTypes

The content types that this channel can deliver.

`xdm:contentTypes`
* is optional
* type: `const`

* defined in this schema

The value of this property **must** be equal to:

```json
[]
```





## xdm:locationTypes

The types of locations (virtual places) that this channel consists of and can deliver content to.

`xdm:locationTypes`
* is optional
* type: `const`

* defined in this schema

The value of this property **must** be equal to:

```json
[]
```





## xdm:mediaAction

The `mediaAction` property is used to provide a type of experiance event media action .

`xdm:mediaAction`
* is optional
* type: `string`
* defined in [Experience Channel](channel.schema.md#xdmmediaaction)

### xdm:mediaAction Type


`string`



### xdm:mediaAction Known Values
| Value | Description |
|-------|-------------|
| `opens` | Opens |
| `sends` | Sends |
| `clicks` | Clicks |
| `impressions` | Impressions |
| `bounces` | Bounces |
| `mirrorpages` | Mirrorpages |
| `nonDeliverables` | NonDeliverables |
| `notSent` | NotSent |
| `offerOpens` | OfferOpens |
| `unSubscriptions` | UnSubscriptions |
| `userComplaints` | UserComplaints |
| `subscriptions` | Subscriptions |




## xdm:mediaType

Describes wether the media type is paid,owned or earned.

`xdm:mediaType`
* is optional
* type: `string`
* defined in [Experience Channel](channel.schema.md#xdmmediatype)

### xdm:mediaType Type


`string`



### xdm:mediaType Known Values
| Value | Description |
|-------|-------------|
| `paid` | Paid |
| `owned` | Owned |
| `earned` | Earned |




## xdm:metricTypes

The metrics that can be collected in this channel.

`xdm:metricTypes`
* is optional
* type: `const`

* defined in this schema

The value of this property **must** be equal to:

```json
[]
```





## xdm:mode

How experiences are delivered in this channel.

`xdm:mode`
* is optional
* type: `const`
* defined in this schema

The value of this property **must** be equal to:

```json
"push"
```


### xdm:mode Known Values
| Value | Description |
|-------|-------------|
| `push` | The publisher of an experience can initiate an experience by sending a message into the channel. Most `push` channels involve some form of subscription or opt-in. |
| `pull` | The consumer can initiate an experience by requesting a location in the channel. Most `pull` channels give publishers some control how the experience is then delivered. |
| `bidirectional` | Both `push` and `pull` interaction modes are supported by the channel. |




## xdm:nameAtSource

Customer defined custom channel name

`xdm:nameAtSource`
* is optional
* type: `string`
* defined in [Experience Channel](channel.schema.md#xdmnameatsource)

### xdm:nameAtSource Type


`string`





