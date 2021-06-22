# Create thread request Schema

```txt
https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/feed/createThread.json
```

Create thread request

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                    |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [createThread.json](../out/api/feed/createThread.json "open original schema") |

## Create thread request Type

`object` ([Create thread request](createthread.md))

# Create thread request Properties

| Property                                | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                          |
| :-------------------------------------- | :------- | :------- | :------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [message](#message)                     | `string` | Required | cannot be null | [Create thread request](createthread-properties-message.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/feed/createThread.json#/properties/message")              |
| [from](#from)                           | `string` | Required | cannot be null | [Create thread request](common-definitions-uuid.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/feed/createThread.json#/properties/from")                         |
| [addressedToEntity](#addressedtoentity) | `object` | Required | cannot be null | [Create thread request](common-definitions-entityreference.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/feed/createThread.json#/properties/addressedToEntity") |

## message

Message

`message`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Create thread request](createthread-properties-message.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/feed/createThread.json#/properties/message")

### message Type

`string`

## from

Unique id used to identify an entity

`from`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Create thread request](common-definitions-uuid.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/feed/createThread.json#/properties/from")

### from Type

`string`

### from Constraints

**UUID**: the string must be a UUID, according to [RFC 4122](https://tools.ietf.org/html/rfc4122 "check the specification")

## addressedToEntity

Entity addressed to which this thread is created

> Entity reference that includes entity ID and entity type

`addressedToEntity`

*   is required

*   Type: `object` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [Create thread request](common-definitions-entityreference.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/feed/createThread.json#/properties/addressedToEntity")

### addressedToEntity Type

`object` ([Details](common-definitions-entityreference.md))
