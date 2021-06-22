# Update Database service entity request Schema

```txt
https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/updateDatabaseService.json
```

Udpate Database service entity request

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                          |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [updateDatabaseService.json](../out/api/services/updateDatabaseService.json "open original schema") |

## Update Database service entity request Type

`object` ([Update Database service entity request](updatedatabaseservice.md))

# Update Database service entity request Properties

| Property                                | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                                                            |
| :-------------------------------------- | :------- | :------- | :------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [description](#description)             | `string` | Optional | cannot be null | [Update Database service entity request](updatedatabaseservice-properties-description.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/updateDatabaseService.json#/properties/description") |
| [jdbc](#jdbc)                           | `object` | Optional | cannot be null | [Update Database service entity request](jdbcconnection-definitions-jdbcinfo.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/updateDatabaseService.json#/properties/jdbc")                 |
| [ingestionSchedule](#ingestionschedule) | `object` | Optional | cannot be null | [Update Database service entity request](common-definitions-schedule.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/updateDatabaseService.json#/properties/ingestionSchedule")            |

## description

Description of Database entity.

`description`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Update Database service entity request](updatedatabaseservice-properties-description.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/updateDatabaseService.json#/properties/description")

### description Type

`string`

## jdbc



> Type for capturing JDBC connector information

`jdbc`

*   is optional

*   Type: `object` ([Details](jdbcconnection-definitions-jdbcinfo.md))

*   cannot be null

*   defined in: [Update Database service entity request](jdbcconnection-definitions-jdbcinfo.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/updateDatabaseService.json#/properties/jdbc")

### jdbc Type

`object` ([Details](jdbcconnection-definitions-jdbcinfo.md))

## ingestionSchedule

Schedule for running metadata ingestion jobs

`ingestionSchedule`

*   is optional

*   Type: `object` ([Details](common-definitions-schedule.md))

*   cannot be null

*   defined in: [Update Database service entity request](common-definitions-schedule.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/services/updateDatabaseService.json#/properties/ingestionSchedule")

### ingestionSchedule Type

`object` ([Details](common-definitions-schedule.md))
