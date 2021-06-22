# Create Database service entity request Schema

```txt
https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/createDatabaseService.json
```

Create Database service entity request

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                          |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [createDatabaseService.json](../out/api/services/createDatabaseService.json "open original schema") |

## Create Database service entity request Type

`object` ([Create Database service entity request](createdatabaseservice.md))

# Create Database service entity request Properties

| Property                                | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                                                               |
| :-------------------------------------- | :------- | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [name](#name)                           | `string` | Required | cannot be null | [Create Database service entity request](createdatabaseservice-properties-name.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/createDatabaseService.json#/properties/name")                  |
| [description](#description)             | `string` | Optional | cannot be null | [Create Database service entity request](createdatabaseservice-properties-description.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/createDatabaseService.json#/properties/description")    |
| [serviceType](#servicetype)             | `string` | Required | cannot be null | [Create Database service entity request](databaseservice-definitions-databaseservicetype.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/createDatabaseService.json#/properties/serviceType") |
| [jdbc](#jdbc)                           | `object` | Required | cannot be null | [Create Database service entity request](jdbcconnection-definitions-jdbcinfo.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/createDatabaseService.json#/properties/jdbc")                    |
| [ingestionSchedule](#ingestionschedule) | `object` | Optional | cannot be null | [Create Database service entity request](common-definitions-schedule.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/createDatabaseService.json#/properties/ingestionSchedule")               |

## name

Name that identifies the this entity instance uniquely

`name`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Create Database service entity request](createdatabaseservice-properties-name.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/createDatabaseService.json#/properties/name")

### name Type

`string`

### name Constraints

**maximum length**: the maximum number of characters for this string is: `64`

**minimum length**: the minimum number of characters for this string is: `1`

## description

Description of Database entity.

`description`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Create Database service entity request](createdatabaseservice-properties-description.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/createDatabaseService.json#/properties/description")

### description Type

`string`

## serviceType

Type of database service such as MySQL, BigQuery, Snowflake, Redshift...

`serviceType`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Create Database service entity request](databaseservice-definitions-databaseservicetype.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/createDatabaseService.json#/properties/serviceType")

### serviceType Type

`string`

### serviceType Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value         | Explanation |
| :------------ | :---------- |
| `"BIGQUERY"`  |             |
| `"MYSQL"`     |             |
| `"REDSHIFT"`  |             |
| `"SNOWFLAKE"` |             |

## jdbc



> Type for capturing JDBC connector information

`jdbc`

*   is required

*   Type: `object` ([Details](jdbcconnection-definitions-jdbcinfo.md))

*   cannot be null

*   defined in: [Create Database service entity request](jdbcconnection-definitions-jdbcinfo.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/createDatabaseService.json#/properties/jdbc")

### jdbc Type

`object` ([Details](jdbcconnection-definitions-jdbcinfo.md))

## ingestionSchedule

Schedule for running metadata ingestion jobs

`ingestionSchedule`

*   is optional

*   Type: `object` ([Details](common-definitions-schedule.md))

*   cannot be null

*   defined in: [Create Database service entity request](common-definitions-schedule.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/createDatabaseService.json#/properties/ingestionSchedule")

### ingestionSchedule Type

`object` ([Details](common-definitions-schedule.md))
