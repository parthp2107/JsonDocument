---
layout: default
title: Classification
---
# Data classification related types Schema

```txt
https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/type/classification.json
```

Data classification related types

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                    |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------------------- |
| Can be instantiated | Yes        | Unknown status | No           | Forbidden         | Allowed               | none                | [classification.json](classification.md) |

## Data classification related types Type

`object` ([Data classification related types](classification.md))

# Data classification related types Properties

| Property      | Type    | Required | Nullable       | Defined by                                                                                                                                                                                                                   |
| :------------ | :------ | :------- | :------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [tags](#tags) | `array` | Optional | cannot be null | [Data classification related types](classification-properties-tags.md) |

## tags



`tags`

*   is optional

*   Type: `object[]` ([Details](classification-definitions-personaldata.md))

*   cannot be null

*   defined in: [Data classification related types](classification-properties-tags.md)

### tags Type

`object[]` ([Details](classification-definitions-personaldata.md))

# Data classification related types Definitions

## Definitions group personalData

Reference this group by using

```json
{"$ref":"https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/type/classification.json#/definitions/personalData"}
```

| Property                              | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                                                                                             |
| :------------------------------------ | :------- | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [name](#name)                         | `string` | Optional | cannot be null | [Data classification related types](classification-definitions-personaldata-properties-name.md)                         |
| [documentation](#documentation)       | `string` | Optional | cannot be null | [Data classification related types](classification-definitions-personaldata-properties-documentation.md)       |
| [piiType](#piitype)                   | `string` | Optional | cannot be null | [Data classification related types](classification-definitions-personaldata-properties-piitype.md)                   |
| [personalDataType](#personaldatatype) | `string` | Optional | cannot be null | [Data classification related types](classification-definitions-personaldata-properties-personaldatatype.md) |

### name

Name of PII tag

`name`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Data classification related types](classification-definitions-personaldata-properties-name.md)

#### name Type

`string`

### documentation

Name of PII tag

`documentation`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Data classification related types](classification-definitions-personaldata-properties-documentation.md)

#### documentation Type

`string`

### piiType

PII tag type

`piiType`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Data classification related types](classification-definitions-personaldata-properties-piitype.md)

#### piiType Type

`string`

#### piiType Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value             | Explanation |
| :---------------- | :---------- |
| `"NONE"`          |             |
| `"NON_SENSITIVE"` |             |
| `"SENSITIVE"`     |             |

### personalDataType

Personal data tag type

`personalDataType`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Data classification related types](classification-definitions-personaldata-properties-personaldatatype.md)

#### personalDataType Type

`string`

#### personalDataType Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                | Explanation |
| :------------------- | :---------- |
| `"PERSONAL"`         |             |
| `"SPECIAL_CATEGORY"` |             |
