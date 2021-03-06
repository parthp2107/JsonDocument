---
layout: default
title: Usage Report
---
# Usage report for an entity Schema

```txt
https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/type/usageReport.json
```

Type used for capturing and reporting usage report of an entity

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                              |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [usageReport.json](usageReport.md) |

## Usage report for an entity Type

`object` ([Usage report for an entity](usagereport.md))

# Usage report for an entity Properties

| Property        | Type      | Required | Nullable       | Defined by                                                                                                                                                                                                        |
| :-------------- | :-------- | :------- | :------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [count](#count) | `integer` | Required | cannot be null | [Usage report for an entity](usagereport-properties-count.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/type/usageReport.json#/properties/count") |
| [date](#date)   | `string`  | Required | cannot be null | [Usage report for an entity](common-definitions-date.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/type/usageReport.json#/properties/date")       |

## count

Usage count of a data asset on the given date

`count`

*   is required

*   Type: `integer`

*   cannot be null

*   defined in: [Usage report for an entity](usagereport-properties-count.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/type/usageReport.json#/properties/count")

### count Type

`integer`

### count Constraints

**minimum**: the value of this number must greater than or equal to: `0`

## date

Date in ISO 8601 format in UTC time. Example - '2018-11-13'

`date`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Usage report for an entity](common-definitions-date.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/type/usageReport.json#/properties/date")

### date Type

`string`

### date Constraints

**date**: the string must be a date string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")
