---
layout: default
title: Team
---
# Team entity Schema

```txt
https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/entity/teams/team.json
```

Team entity

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                        |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [team.json](team.md) |

## Team entity Type

`object` ([Team entity](team.md))

# Team entity Properties

| Property                    | Type      | Required | Nullable       | Defined by                                                                                                                                                                                                    |
| :-------------------------- | :-------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [id](#id)                   | `string`  | Required | cannot be null | [Team entity](common-definitions-uuid.md)                   |
| [name](#name)               | `string`  | Required | cannot be null | [Team entity](team-properties-name.md)                    |
| [displayName](#displayname) | `string`  | Optional | cannot be null | [Team entity](team-properties-displayname.md)      |
| [description](#description) | `string`  | Optional | cannot be null | [Team entity](team-properties-description.md)      |
| [href](#href)               | `string`  | Required | cannot be null | [Team entity](common-definitions-href.md)                 |
| [profile](#profile)         | `object`  | Optional | cannot be null | [Team entity](common-definitions-profile.md)           |
| [deleted](#deleted)         | `boolean` | Optional | cannot be null | [Team entity](team-properties-deleted.md)              |
| [users](#users)             | `array`   | Optional | cannot be null | [Team entity](common-definitions-entityreferencelist.md) |
| [owns](#owns)               | `array`   | Optional | cannot be null | [Team entity](common-definitions-entityreferencelist.md)  |

## id

Unique id used to identify an entity

`id`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Team entity](common-definitions-uuid.md)

### id Type

`string`

### id Constraints

**UUID**: the string must be a UUID, according to [RFC 4122](https://tools.ietf.org/html/rfc4122 "check the specification")

## name

Unique name that identifies the team

`name`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Team entity](team-properties-name.md)

### name Type

`string`

### name Constraints

**maximum length**: the maximum number of characters for this string is: `64`

**minimum length**: the minimum number of characters for this string is: `1`

## displayName

Name used for display purposes. Example 'Data Science team'

`displayName`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Team entity](team-properties-displayname.md)

### displayName Type

`string`

## description

Description of the team

`description`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Team entity](team-properties-description.md)

### description Type

`string`

## href

Link to the resource corresponding to this entity

> Link to the resource

`href`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Team entity](common-definitions-href.md)

### href Type

`string`

### href Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc3986 "check the specification")

## profile

Team profile information

> Profile of a user, team, or an organization

`profile`

*   is optional

*   Type: `object` ([Details](common-definitions-profile.md))

*   cannot be null

*   defined in: [Team entity](common-definitions-profile.md)

### profile Type

`object` ([Details](common-definitions-profile.md))

## deleted



`deleted`

*   is optional

*   Type: `boolean`

*   cannot be null

*   defined in: [Team entity](team-properties-deleted.md)

### deleted Type

`boolean`

## users

Users that are part of the team

`users`

*   is optional

*   Type: `object[]` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [Team entity](common-definitions-entityreferencelist.md)

### users Type

`object[]` ([Details](common-definitions-entityreference.md))

## owns

Entities owned by the team

`owns`

*   is optional

*   Type: `object[]` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [Team entity](common-definitions-entityreferencelist.md)

### owns Type

`object[]` ([Details](common-definitions-entityreference.md))
