---
layout: default
title: Database
---
# Database entity Schema

```txt
https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/entity/data/database.json
```

Entity that represents a database

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                               |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :----------------------------------------------------------------------- |
| Can be instantiated | Yes        | Unknown status | No           | Forbidden         | Allowed               | none                | [database.json](database.md) |

## Database entity Type

`object` ([Database entity](database.md))

# Database entity Properties

| Property                                  | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                        |
| :---------------------------------------- | :------- | :------- | :------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id)                                 | `string` | Optional | cannot be null | [Database entity](common-definitions-uuid.md)                                |
| [name](#name)                             | `string` | Required | cannot be null | [Database entity](database-properties-name.md)                             |
| [fullyQualifiedName](#fullyqualifiedname) | `string` | Optional | cannot be null | [Database entity](database-properties-fullyqualifiedname.md) |
| [description](#description)               | `string` | Optional | cannot be null | [Database entity](database-properties-description.md)               |
| [href](#href)                             | `string` | Optional | cannot be null | [Database entity](common-definitions-href.md)                              |
| [owner](#owner)                           | `object` | Optional | cannot be null | [Database entity](common-definitions-entityreference.md)                  |
| [service](#service)                       | `object` | Required | cannot be null | [Database entity](common-definitions-entityreference.md)                |
| [usageSummary](#usagesummary)             | `object` | Optional | cannot be null | [Database entity](common-definitions-usagedetails.md )              |
| [tables](#tables)                         | `array`  | Optional | cannot be null | [Database entity](common-definitions-entityreferencelist.md)             |

## id

Unique id used to identify an entity

`id`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Database entity](common-definitions-uuid.md)

### id Type

`string`

### id Constraints

**UUID**: the string must be a UUID, according to [RFC 4122](https://tools.ietf.org/html/rfc4122 "check the specification")

## name

Name that identifies the database

`name`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Database entity](database-properties-name.md)

### name Type

`string`

### name Constraints

**maximum length**: the maximum number of characters for this string is: `64`

**minimum length**: the minimum number of characters for this string is: `1`

**pattern**: the string must match the following regular expression: 

```regexp
^[^.]*$
```

[try pattern](https://regexr.com/?expression=%5E%5B%5E.%5D\*%24 "try regular expression with regexr.com")

## fullyQualifiedName

Name that uniquely identifies a database in the format 'ServiceName.DatabaseName'

`fullyQualifiedName`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Database entity](database-properties-fullyqualifiedname.md)

### fullyQualifiedName Type

`string`

## description

Description of the database instance. What it has and how to use it.

`description`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Database entity](database-properties-description.md)

### description Type

`string`

## href

Link to the resource corresponding to this entity

> Link to the resource

`href`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Database entity](common-definitions-href.md)

### href Type

`string`

### href Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc3986 "check the specification")

## owner

Owner of this database

> Entity reference that includes entity ID and entity type

`owner`

*   is optional

*   Type: `object` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [Database entity](common-definitions-entityreference.md)

### owner Type

`object` ([Details](common-definitions-entityreference.md))

## service

Link to the database cluster/service where this database is hosted in

> Entity reference that includes entity ID and entity type

`service`

*   is required

*   Type: `object` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [Database entity](common-definitions-entityreference.md)

### service Type

`object` ([Details](common-definitions-entityreference.md))

## usageSummary

Latest usage information for this database

> Type used to return usage details

`usageSummary`

*   is optional

*   Type: `object` ([Details](common-definitions-usagedetails.md))

*   cannot be null

*   defined in: [Database entity](common-definitions-usagedetails.md )

### usageSummary Type

`object` ([Details](common-definitions-usagedetails.md))

## tables

References to tables in the database

`tables`

*   is optional

*   Type: `object[]` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [Database entity](common-definitions-entityreferencelist.md)

### tables Type

`object[]` ([Details](common-definitions-entityreference.md))

# Database entity Definitions

## Definitions group databaseName

Reference this group by using

```json
{"$ref":"https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/entity/data/database.json#/definitions/databaseName"}
```

| Property | Type | Required | Nullable | Defined by |
| :------- | :--- | :------- | :------- | :--------- |
