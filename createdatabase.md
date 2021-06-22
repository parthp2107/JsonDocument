# Create Database entity request Schema

```txt
https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createDatabase.json
```

Create Database entity request

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                        |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [createDatabase.json](../out/api/data/createDatabase.json "open original schema") |

## Create Database entity request Type

`object` ([Create Database entity request](createdatabase.md))

# Create Database entity request Properties

| Property                    | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                                  |
| :-------------------------- | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [name](#name)               | `string` | Required | cannot be null | [Create Database entity request](database-definitions-databasename.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createDatabase.json#/properties/name")            |
| [description](#description) | `string` | Optional | cannot be null | [Create Database entity request](createdatabase-properties-description.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createDatabase.json#/properties/description") |
| [owner](#owner)             | `object` | Optional | cannot be null | [Create Database entity request](common-definitions-entityreference.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createDatabase.json#/properties/owner")          |
| [service](#service)         | `object` | Required | cannot be null | [Create Database entity request](common-definitions-entityreference.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createDatabase.json#/properties/service")        |

## name

Name that identifies the database

`name`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Create Database entity request](database-definitions-databasename.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createDatabase.json#/properties/name")

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

## description

Description of the database instance. What it has and how to use it.

`description`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Create Database entity request](createdatabase-properties-description.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createDatabase.json#/properties/description")

### description Type

`string`

## owner

Owner of this database

> Entity reference that includes entity ID and entity type

`owner`

*   is optional

*   Type: `object` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [Create Database entity request](common-definitions-entityreference.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createDatabase.json#/properties/owner")

### owner Type

`object` ([Details](common-definitions-entityreference.md))

## service

Link to the database service where this database is hosted in

> Entity reference that includes entity ID and entity type

`service`

*   is required

*   Type: `object` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [Create Database entity request](common-definitions-entityreference.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createDatabase.json#/properties/service")

### service Type

`object` ([Details](common-definitions-entityreference.md))
