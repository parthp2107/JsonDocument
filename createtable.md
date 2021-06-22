# Table entity Schema

```txt
https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json
```

Schema corresponding to a table that belongs to a database

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                  |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [createTable.json](../out/api/data/createTable.json "open original schema") |

## Table entity Type

`object` ([Table entity](createtable.md))

# Table entity Properties

| Property                              | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                    |
| :------------------------------------ | :------- | :------- | :------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [name](#name)                         | `string` | Required | cannot be null | [Table entity](table-definitions-tablename.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json#/properties/name")                         |
| [description](#description)           | `string` | Optional | cannot be null | [Table entity](createtable-properties-description.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json#/properties/description")           |
| [tableType](#tabletype)               | `string` | Optional | cannot be null | [Table entity](table-definitions-tabletype.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json#/properties/tableType")                    |
| [columns](#columns)                   | `array`  | Required | cannot be null | [Table entity](createtable-properties-columns.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json#/properties/columns")                   |
| [tableConstraints](#tableconstraints) | `array`  | Optional | cannot be null | [Table entity](createtable-properties-tableconstraints.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json#/properties/tableConstraints") |
| [owner](#owner)                       | `object` | Optional | cannot be null | [Table entity](common-definitions-entityreference.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json#/properties/owner")                 |
| [database](#database)                 | `string` | Required | cannot be null | [Table entity](common-definitions-uuid.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json#/properties/database")                         |
| [tags](#tags)                         | `array`  | Optional | cannot be null | [Table entity](createtable-properties-tags.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json#/properties/tags")                         |

## name

Local name (not fully qualified name) of the table

`name`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](table-definitions-tablename.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json#/properties/name")

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

Description of entity instance.

`description`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](createtable-properties-description.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json#/properties/description")

### description Type

`string`

## tableType

Type for capturing a column in a table

`tableType`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](table-definitions-tabletype.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json#/properties/tableType")

### tableType Type

`string`

### tableType Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                 | Explanation |
| :-------------------- | :---------- |
| `"REGULAR"`           |             |
| `"EXTERNAL"`          |             |
| `"VIEW"`              |             |
| `"SECURE_VIEW"`       |             |
| `"MATERIALIZED_VIEW"` |             |

## columns

Name of the tables in the database

`columns`

*   is required

*   Type: `object[]` ([Details](table-definitions-column.md))

*   cannot be null

*   defined in: [Table entity](createtable-properties-columns.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json#/properties/columns")

### columns Type

`object[]` ([Details](table-definitions-column.md))

## tableConstraints



`tableConstraints`

*   is optional

*   Type: `object[]` ([Details](table-definitions-tableconstraint.md))

*   cannot be null

*   defined in: [Table entity](createtable-properties-tableconstraints.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json#/properties/tableConstraints")

### tableConstraints Type

`object[]` ([Details](table-definitions-tableconstraint.md))

## owner

Owner of this entity

> Entity reference that includes entity ID and entity type

`owner`

*   is optional

*   Type: `object` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [Table entity](common-definitions-entityreference.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json#/properties/owner")

### owner Type

`object` ([Details](common-definitions-entityreference.md))

## database

Unique id used to identify an entity

`database`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](common-definitions-uuid.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json#/properties/database")

### database Type

`string`

### database Constraints

**UUID**: the string must be a UUID, according to [RFC 4122](https://tools.ietf.org/html/rfc4122 "check the specification")

## tags

Tags for this table

`tags`

*   is optional

*   Type: `object[]` ([Details](common-definitions-taglabel.md))

*   cannot be null

*   defined in: [Table entity](createtable-properties-tags.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/data/createTable.json#/properties/tags")

### tags Type

`object[]` ([Details](common-definitions-taglabel.md))
