---
layout: default
title: Table
---
# Table entity Schema

```txt
https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/entity/data/table.json
```

Schema corresponding to a table that belongs to a database

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                         |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :----------------------------------------------------------------- |
| Can be instantiated | Yes        | Unknown status | No           | Forbidden         | Allowed               | none                | [table.json](table.md) |

## Table entity Type

`object` ([Table entity](table.md))

# Table entity Properties

| Property                                  | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                               |
| :---------------------------------------- | :------- | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id)                                 | `string` | Optional | cannot be null | [Table entity](common-definitions-uuid.md)                             |
| [name](#name)                             | `string` | Required | cannot be null | [Table entity](table-properties-name.md)                             |
| [description](#description)               | `string` | Optional | cannot be null | [Table entity](table-properties-description.md)               |
| [href](#href)                             | `string` | Optional | cannot be null | [Table entity](common-definitions-href.md)                           |
| [tableType](#tabletype)                   | `string` | Optional | cannot be null | [Table entity](table-properties-tabletype.md)                   |
| [fullyQualifiedName](#fullyqualifiedname) | `string` | Optional | cannot be null | [Table entity](table-properties-fullyqualifiedname.md) |
| [columns](#columns)                       | `array`  | Required | cannot be null | [Table entity](table-properties-columns.md)                       |
| [tableConstraints](#tableconstraints)     | `array`  | Optional | cannot be null | [Table entity](table-properties-tableconstraints.md)     |
| [usageSummary](#usagesummary)             | `object` | Optional | cannot be null | [Table entity](common-definitions-usagedetails.md)           |
| [owner](#owner)                           | `object` | Optional | cannot be null | [Table entity](common-definitions-entityreference.md)               |
| [followers](#followers)                   | `array`  | Optional | cannot be null | [Table entity](common-definitions-entityreferencelist.md)       |
| [database](#database)                     | `object` | Optional | cannot be null | [Table entity](common-definitions-entityreference.md)            |
| [tags](#tags)                             | `array`  | Optional | cannot be null | [Table entity](table-properties-tags.md)                             |
| [joins](#joins)                           | `array`  | Optional | cannot be null | [Table entity](table-properties-joins.md)                           |
| [sampleData](#sampledata)                 | `object` | Optional | cannot be null | [Table entity](table-definitions-tabledata.md)                 |

## id

Unique id used to identify an entity

`id`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](common-definitions-uuid.md)

### id Type

`string`

### id Constraints

**UUID**: the string must be a UUID, according to [RFC 4122](https://tools.ietf.org/html/rfc4122 "check the specification")

## name

Local name (not fully qualified name) of the table

`name`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](table-properties-name.md)

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

Description of the table

`description`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](table-properties-description.md)

### description Type

`string`

## href

Link to this table resource

> Link to the resource

`href`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](common-definitions-href.md)

### href Type

`string`

### href Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc3986 "check the specification")

## tableType

Type for capturing a column in a table

`tableType`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](table-properties-tabletype.md)

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

## fullyQualifiedName

Fully qualified name of the table in the form serviceName.databaseName.tableName

`fullyQualifiedName`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](table-properties-fullyqualifiedname.md)

### fullyQualifiedName Type

`string`

## columns

Columns in the table

`columns`

*   is required

*   Type: `object[]` ([Details](table-definitions-column.md))

*   cannot be null

*   defined in: [Table entity](table-properties-columns.md)

### columns Type

`object[]` ([Details](table-definitions-column.md))

## tableConstraints



`tableConstraints`

*   is optional

*   Type: `object[]` ([Details](table-definitions-tableconstraint.md))

*   cannot be null

*   defined in: [Table entity](table-properties-tableconstraints.md)

### tableConstraints Type

`object[]` ([Details](table-definitions-tableconstraint.md))

## usageSummary

Latest usage information for this table

> Type used to return usage details

`usageSummary`

*   is optional

*   Type: `object` ([Details](common-definitions-usagedetails.md))

*   cannot be null

*   defined in: [Table entity](common-definitions-usagedetails.md)

### usageSummary Type

`object` ([Details](common-definitions-usagedetails.md))

## owner

Owner of this table

> Entity reference that includes entity ID and entity type

`owner`

*   is optional

*   Type: `object` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [Table entity](common-definitions-entityreference.md)

### owner Type

`object` ([Details](common-definitions-entityreference.md))

## followers

Followers of this table

`followers`

*   is optional

*   Type: `object[]` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [Table entity](common-definitions-entityreferencelist.md)

### followers Type

`object[]` ([Details](common-definitions-entityreference.md))

## database

Reference to Database that contains this table

> Entity reference that includes entity ID and entity type

`database`

*   is optional

*   Type: `object` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [Table entity](common-definitions-entityreference.md)

### database Type

`object` ([Details](common-definitions-entityreference.md))

## tags

Tags for this table

`tags`

*   is optional

*   Type: `object[]` ([Details](common-definitions-taglabel.md))

*   cannot be null

*   defined in: [Table entity](table-properties-tags.md)

### tags Type

`object[]` ([Details](common-definitions-taglabel.md))

## joins

Details of other tables this table is frequently joined with

`joins`

*   is optional

*   Type: `object[]` ([Details](table-definitions-columnjoin.md))

*   cannot be null

*   defined in: [Table entity](table-properties-joins.md)

### joins Type

`object[]` ([Details](table-definitions-columnjoin.md))

## sampleData

Information on other tables that this table column is frequently joined with

`sampleData`

*   is optional

*   Type: `object` ([Details](table-definitions-tabledata.md))

*   cannot be null

*   defined in: [Table entity](table-definitions-tabledata.md)

### sampleData Type

`object` ([Details](table-definitions-tabledata.md))

# Table entity Definitions

## Definitions group tableType

Reference this group by using

```json
{"$ref":"https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/entity/data/table.json#/definitions/tableType"}
```

| Property | Type | Required | Nullable | Defined by |
| :------- | :--- | :------- | :------- | :--------- |

## Definitions group columnDataType

Reference this group by using

```json
{"$ref":"https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/entity/data/table.json#/definitions/columnDataType"}
```

| Property | Type | Required | Nullable | Defined by |
| :------- | :--- | :------- | :------- | :--------- |

## Definitions group columnConstraint

Reference this group by using

```json
{"$ref":"https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/entity/data/table.json#/definitions/columnConstraint"}
```

| Property | Type | Required | Nullable | Defined by |
| :------- | :--- | :------- | :------- | :--------- |

## Definitions group tableConstraint

Reference this group by using

```json
{"$ref":"https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/entity/data/table.json#/definitions/tableConstraint"}
```

| Property                          | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                                                               |
| :-------------------------------- | :------- | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [constraintType](#constrainttype) | `string` | Optional | cannot be null | [Table entity](table-definitions-tableconstraint-properties-constrainttype.md) |
| [columns](#columns-1)             | `array`  | Optional | cannot be null | [Table entity](table-definitions-tableconstraint-properties-columns.md)               |

### constraintType



`constraintType`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](table-definitions-tableconstraint-properties-constrainttype.md)

#### constraintType Type

`string`

#### constraintType Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value           | Explanation |
| :-------------- | :---------- |
| `"UNIQUE"`      |             |
| `"PRIMARY_KEY"` |             |
| `"FOREIGN_KEY"` |             |

### columns

List of column names corresponding to the constraint

`columns`

*   is optional

*   Type: `string[]`

*   cannot be null

*   defined in: [Table entity](table-definitions-tableconstraint-properties-columns.md)

#### columns Type

`string[]`

## Definitions group columnName

Reference this group by using

```json
{"$ref":"https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/entity/data/table.json#/definitions/columnName"}
```

| Property | Type | Required | Nullable | Defined by |
| :------- | :--- | :------- | :------- | :--------- |

## Definitions group tableName

Reference this group by using

```json
{"$ref":"https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/entity/data/table.json#/definitions/tableName"}
```

| Property | Type | Required | Nullable | Defined by |
| :------- | :--- | :------- | :------- | :--------- |

## Definitions group fullyQualifiedColumnName

Reference this group by using

```json
{"$ref":"https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/entity/data/table.json#/definitions/fullyQualifiedColumnName"}
```

| Property | Type | Required | Nullable | Defined by |
| :------- | :--- | :------- | :------- | :--------- |

## Definitions group column

Reference this group by using

```json
{"$ref":"https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/entity/data/table.json#/definitions/column"}
```

| Property                                    | Type      | Required | Nullable       | Defined by                                                                                                                                                                                                                                                     |
| :------------------------------------------ | :-------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [name](#name-1)                             | `string`  | Required | cannot be null | [Table entity](table-definitions-column-properties-name.md)                             |
| [columnDataType](#columndatatype)           | `string`  | Required | cannot be null | [Table entity](table-definitions-column-properties-columndatatype.md)         |
| [description](#description-1)               | `string`  | Optional | cannot be null | [Table entity](table-definitions-column-properties-description.md)               |
| [fullyQualifiedName](#fullyqualifiedname-1) | `string`  | Optional | cannot be null | [Table entity](table-definitions-column-properties-fullyqualifiedname.md) |
| [tags](#tags-1)                             | `array`   | Optional | cannot be null | [Table entity](table-definitions-column-properties-tags.md)                             |
| [columnConstraint](#columnconstraint)       | `string`  | Optional | cannot be null | [Table entity](table-definitions-column-properties-columnconstraint.md)     |
| [ordinalPosition](#ordinalposition)         | `integer` | Optional | cannot be null | [Table entity](table-definitions-column-properties-ordinalposition.md)       |

### name

Local name (not fully qualified name) of the column

`name`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](table-definitions-column-properties-name.md)

#### name Type

`string`

#### name Constraints

**maximum length**: the maximum number of characters for this string is: `64`

**minimum length**: the minimum number of characters for this string is: `1`

**pattern**: the string must match the following regular expression: 

```regexp
^[^.]*$
```

[try pattern](https://regexr.com/?expression=%5E%5B%5E.%5D\*%24 "try regular expression with regexr.com")

### columnDataType

Type for capturing a column in a table

`columnDataType`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](table-definitions-column-properties-columndatatype.md)

#### columnDataType Type

`string`

#### columnDataType Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value          | Explanation |
| :------------- | :---------- |
| `"NUMBER"`     |             |
| `"TINYINT"`    |             |
| `"SMALLINT"`   |             |
| `"INT"`        |             |
| `"BIGINT"`     |             |
| `"FLOAT"`      |             |
| `"DOUBLE"`     |             |
| `"DECIMAL"`    |             |
| `"NUMERIC"`    |             |
| `"TIMESTAMP"`  |             |
| `"TIME"`       |             |
| `"DATE"`       |             |
| `"DATETIME"`   |             |
| `"INTERVAL"`   |             |
| `"STRING"`     |             |
| `"MEDIUMTEXT"` |             |
| `"TEXT"`       |             |
| `"CHAR"`       |             |
| `"VARCHAR"`    |             |
| `"BOOLEAN"`    |             |
| `"BINARY"`     |             |
| `"VARBINARY"`  |             |
| `"ARRAY"`      |             |
| `"BLOB"`       |             |
| `"LONGBLOB"`   |             |
| `"MEDIUMBLOB"` |             |
| `"MAP"`        |             |
| `"STRUCT"`     |             |
| `"UNION"`      |             |
| `"SET"`        |             |
| `"GEOGRAPHY"`  |             |
| `"ENUM"`       |             |
| `"JSON"`       |             |

### description

Description of the column

`description`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](table-definitions-column-properties-description.md)

#### description Type

`string`

### fullyQualifiedName

Fully qualified name of the column that includes serviceName.databaseName.tableName.columnName

`fullyQualifiedName`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](table-definitions-column-properties-fullyqualifiedname.md)

#### fullyQualifiedName Type

`string`

#### fullyQualifiedName Constraints

**maximum length**: the maximum number of characters for this string is: `256`

**minimum length**: the minimum number of characters for this string is: `1`

### tags

Tags associated with the column

`tags`

*   is optional

*   Type: `object[]` ([Details](common-definitions-taglabel.md))

*   cannot be null

*   defined in: [Table entity](table-definitions-column-properties-tags.md)

#### tags Type

`object[]` ([Details](common-definitions-taglabel.md))

### columnConstraint

Column constraint

`columnConstraint`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](table-definitions-column-properties-columnconstraint.md)

#### columnConstraint Type

`string`

#### columnConstraint Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value           | Explanation |
| :-------------- | :---------- |
| `"NULL"`        |             |
| `"NOT_NULL"`    |             |
| `"UNIQUE"`      |             |
| `"PRIMARY_KEY"` |             |

#### columnConstraint Default Value

The default value is:

```json
"NULL"
```

### ordinalPosition

Ordinal position of the column

`ordinalPosition`

*   is optional

*   Type: `integer`

*   cannot be null

*   defined in: [Table entity](table-definitions-column-properties-ordinalposition.md)

#### ordinalPosition Type

`integer`

## Definitions group columnJoin

Reference this group by using

```json
{"$ref":"https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/entity/data/table.json#/definitions/columnJoin"}
```

| Property                  | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                                             |
| :------------------------ | :------- | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [columnName](#columnname) | `string` | Optional | cannot be null | [Table entity](table-definitions-columnjoin-properties-columnname.md) |
| [joinedWith](#joinedwith) | `array`  | Optional | cannot be null | [Table entity](table-definitions-columnjoin-properties-joinedwith.md) |

### columnName

Local name (not fully qualified name) of the column

`columnName`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Table entity](table-definitions-columnjoin-properties-columnname.md)

#### columnName Type

`string`

#### columnName Constraints

**maximum length**: the maximum number of characters for this string is: `64`

**minimum length**: the minimum number of characters for this string is: `1`

**pattern**: the string must match the following regular expression: 

```regexp
^[^.]*$
```

[try pattern](https://regexr.com/?expression=%5E%5B%5E.%5D\*%24 "try regular expression with regexr.com")

### joinedWith

Fully qualified names of the columns that this column is joined with

`joinedWith`

*   is optional

*   Type: `string[]`

*   cannot be null

*   defined in: [Table entity](table-definitions-columnjoin-properties-joinedwith.md)

#### joinedWith Type

`string[]`

## Definitions group tableData

Reference this group by using

```json
{"$ref":"https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/entity/data/table.json#/definitions/tableData"}
```

| Property              | Type    | Required | Nullable       | Defined by                                                                                                                                                                                                                                     |
| :-------------------- | :------ | :------- | :------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [columns](#columns-2) | `array` | Optional | cannot be null | [Table entity](table-definitions-tabledata-properties-columns.md) |
| [rows](#rows)         | `array` | Optional | cannot be null | [Table entity](table-definitions-tabledata-properties-rows.md)       |

### columns



`columns`

*   is optional

*   Type: `string[]`

*   cannot be null

*   defined in: [Table entity](table-definitions-tabledata-properties-columns.md)

#### columns Type

`string[]`

### rows

Data for a multiple rows of the table

`rows`

*   is optional

*   Type: `array[]`

*   cannot be null

*   defined in: [Table entity](table-definitions-tabledata-properties-rows.md)

#### rows Type

`array[]`
