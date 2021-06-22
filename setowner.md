# Set ownership for a given entity Schema

```txt
https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/setOwner.json
```

Set ownership for a given entity

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                       |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :--------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [setOwner.json](../out/api/setOwner.json "open original schema") |

## Set ownership for a given entity Type

`object` ([Set ownership for a given entity](setowner.md))

# Set ownership for a given entity Properties

| Property      | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                     |
| :------------ | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id)     | `string` | Optional | cannot be null | [Set ownership for a given entity](common-definitions-uuid.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/setOwner.json#/properties/id")    |
| [type](#type) | `string` | Optional | cannot be null | [Set ownership for a given entity](setowner-properties-type.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/setOwner.json#/properties/type") |

## id

Unique id used to identify an entity

`id`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Set ownership for a given entity](common-definitions-uuid.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/setOwner.json#/properties/id")

### id Type

`string`

### id Constraints

**UUID**: the string must be a UUID, according to [RFC 4122](https://tools.ietf.org/html/rfc4122 "check the specification")

## type

Entity type of the owner typically either 'user' or 'team'

`type`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Set ownership for a given entity](setowner-properties-type.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/setOwner.json#/properties/type")

### type Type

`string`
