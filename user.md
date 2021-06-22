---
layout: default
title: User
---
# User entity Schema

```txt
https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/entity/teams/user.json
```

User entity that is part of an organization

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                        |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [user.json](user.md) |

## User entity Type

`object` ([User entity](user.md))

# User entity Properties

| Property                    | Type      | Required | Nullable       | Defined by                                                                                                                                                                                                      |
| :-------------------------- | :-------- | :------- | :------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id)                   | `string`  | Required | cannot be null | [User entity](common-definitions-uuid.md)                     |
| [name](#name)               | `string`  | Required | cannot be null | [User entity](user-properties-name.md)                      |
| [displayName](#displayname) | `string`  | Optional | cannot be null | [User entity](user-properties-displayname.md)        |
| [href](#href)               | `string`  | Required | cannot be null | [User entity](common-definitions-href.md)                   |
| [timezone](#timezone)       | `string`  | Optional | cannot be null | [User entity](user-properties-timezone.md)              |
| [deleted](#deleted)         | `boolean` | Optional | cannot be null | [User entity](user-properties-deleted.md)                |
| [isBot](#isbot)             | `boolean` | Optional | cannot be null | [User entity](user-properties-isbot.md)                    |
| [profile](#profile)         | `object`  | Optional | cannot be null | [User entity](common-definitions-profile.md)             |
| [teams](#teams)             | `array`   | Optional | cannot be null | [User entity](common-definitions-entityreferencelist.md)   |
| [owns](#owns)               | `array`   | Optional | cannot be null | [User entity](common-definitions-entityreferencelist.md)    |
| [follows](#follows)         | `array`   | Optional | cannot be null | [User entity](common-definitions-entityreferencelist.md) |

## id

Unique id used to identify an entity

`id`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [User entity](common-definitions-uuid.md)

### id Type

`string`

### id Constraints

**UUID**: the string must be a UUID, according to [RFC 4122](https://tools.ietf.org/html/rfc4122 "check the specification")

## name

Name that identifies the this entity instance uniquely. Same as id if when name is not unique

`name`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [User entity](user-properties-name.md)

### name Type

`string`

### name Constraints

**maximum length**: the maximum number of characters for this string is: `64`

**minimum length**: the minimum number of characters for this string is: `1`

## displayName

Name used for display purposes. Example 'FirstName LastName'

`displayName`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [User entity](user-properties-displayname.md)

### displayName Type

`string`

## href

Link to the resource corresponding to this entity

> Link to the resource

`href`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [User entity](common-definitions-href.md)

### href Type

`string`

### href Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc3986 "check the specification")

## timezone

Timezone of the user

`timezone`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [User entity](user-properties-timezone.md)

### timezone Type

`string`

### timezone Constraints

**unknown format**: the value of this string must follow the format: `timezone`

## deleted



`deleted`

*   is optional

*   Type: `boolean`

*   cannot be null

*   defined in: [User entity](user-properties-deleted.md)

### deleted Type

`boolean`

## isBot



`isBot`

*   is optional

*   Type: `boolean`

*   cannot be null

*   defined in: [User entity](user-properties-isbot.md)

### isBot Type

`boolean`

## profile



> Profile of a user, team, or an organization

`profile`

*   is optional

*   Type: `object` ([Details](common-definitions-profile.md))

*   cannot be null

*   defined in: [User entity](common-definitions-profile.md)

### profile Type

`object` ([Details](common-definitions-profile.md))

## teams

Teams that the user belongs to

`teams`

*   is optional

*   Type: `object[]` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [User entity](common-definitions-entityreferencelist.md)

### teams Type

`object[]` ([Details](common-definitions-entityreference.md))

## owns

Entities owned by the user

`owns`

*   is optional

*   Type: `object[]` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [User entity](common-definitions-entityreferencelist.md)

### owns Type

`object[]` ([Details](common-definitions-entityreference.md))

## follows

Entities followed by the user

`follows`

*   is optional

*   Type: `object[]` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [User entity](common-definitions-entityreferencelist.md)

### follows Type

`object[]` ([Details](common-definitions-entityreference.md))
