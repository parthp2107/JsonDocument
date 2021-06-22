---
layout: default
title: Metrics
---
# Metrics entity Schema

```txt
https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/entity/data/metrics.json
```

Entity that represents a Metrics

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                             |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :--------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [metrics.json](metrics.md) |

## Metrics entity Type

`object` ([Metrics entity](metrics.md))

# Metrics entity Properties

| Property                                  | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                     |
| :---------------------------------------- | :------- | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id)                                 | `string` | Required | cannot be null | [Metrics entity](common-definitions-uuid.md)                               |
| [name](#name)                             | `string` | Required | cannot be null | [Metrics entity](metrics-properties-name.md)                             |
| [fullyQualifiedName](#fullyqualifiedname) | `string` | Optional | cannot be null | [Metrics entity](metrics-properties-fullyqualifiedname.md) |
| [description](#description)               | `string` | Optional | cannot be null | [Metrics entity](metrics-properties-description.md)               |
| [href](#href)                             | `string` | Optional | cannot be null | [Metrics entity](common-definitions-href.md)                             |
| [owner](#owner)                           | `object` | Optional | cannot be null | [Metrics entity](common-definitions-entityreference.md)                 |
| [service](#service)                       | `object` | Required | cannot be null | [Metrics entity](common-definitions-entityreference.md)               |
| [usageSummary](#usagesummary)             | `object` | Optional | cannot be null | [Metrics entity](common-definitions-usagedetails.md)             |

## id

Unique id used to identify an entity

`id`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Metrics entity](common-definitions-uuid.md)

### id Type

`string`

### id Constraints

**UUID**: the string must be a UUID, according to [RFC 4122](https://tools.ietf.org/html/rfc4122 "check the specification")

## name

Name that identifies the this metrics instance uniquely.

`name`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Metrics entity](metrics-properties-name.md)

### name Type

`string`

### name Constraints

**maximum length**: the maximum number of characters for this string is: `64`

**minimum length**: the minimum number of characters for this string is: `1`

## fullyQualifiedName

Unique name that identifies a metric in the format 'ServiceName.MetricName'

`fullyQualifiedName`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Metrics entity](metrics-properties-fullyqualifiedname.md)

### fullyQualifiedName Type

`string`

### fullyQualifiedName Constraints

**maximum length**: the maximum number of characters for this string is: `64`

**minimum length**: the minimum number of characters for this string is: `1`

## description

Description of metrics instance. What is has and how to use it

`description`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Metrics entity](metrics-properties-description.md)

### description Type

`string`

## href

Link to the resource corresponding to this entity

> Link to the resource

`href`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Metrics entity](common-definitions-href.md)

### href Type

`string`

### href Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc3986 "check the specification")

## owner

Owner of this metrics

> Entity reference that includes entity ID and entity type

`owner`

*   is optional

*   Type: `object` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [Metrics entity](common-definitions-entityreference.md)

### owner Type

`object` ([Details](common-definitions-entityreference.md))

## service

Link to service where this metrics is hosted in

> Entity reference that includes entity ID and entity type

`service`

*   is required

*   Type: `object` ([Details](common-definitions-entityreference.md))

*   cannot be null

*   defined in: [Metrics entity](common-definitions-entityreference.md)

### service Type

`object` ([Details](common-definitions-entityreference.md))

## usageSummary

Latest usage information for this database

> Type used to return usage details

`usageSummary`

*   is optional

*   Type: `object` ([Details](common-definitions-usagedetails.md))

*   cannot be null

*   defined in: [Metrics entity](common-definitions-usagedetails.md)

### usageSummary Type

`object` ([Details](common-definitions-usagedetails.md))
