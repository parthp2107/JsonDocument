# Create tag category request Schema

```txt
https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/tags/createTagCategory.json
```

Create tag category request

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                              |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [createTagCategory.json](../out/api/tags/createTagCategory.json "open original schema") |

## Create tag category request Type

`object` ([Create tag category request](createtagcategory.md))

# Create tag category request Properties

| Property                      | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                                     |
| :---------------------------- | :------- | :------- | :------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [name](#name)                 | `string` | Required | cannot be null | [Create tag category request](tagcategory-definitions-tagname.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/tags/createTagCategory.json#/properties/name")                 |
| [description](#description)   | `string` | Required | cannot be null | [Create tag category request](createtagcategory-properties-description.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/tags/createTagCategory.json#/properties/description") |
| [categoryType](#categorytype) | `string` | Optional | cannot be null | [Create tag category request](tagcategory-definitions-tagcategorytype.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/tags/createTagCategory.json#/properties/categoryType") |

## name

Name of the tag

`name`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Create tag category request](tagcategory-definitions-tagname.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/tags/createTagCategory.json#/properties/name")

### name Type

`string`

### name Constraints

**maximum length**: the maximum number of characters for this string is: `25`

**minimum length**: the minimum number of characters for this string is: `2`

## description

Description of the tag category

`description`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Create tag category request](createtagcategory-properties-description.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/tags/createTagCategory.json#/properties/description")

### description Type

`string`

## categoryType

Type of tag category

`categoryType`

*   is optional

*   Type: `string`

*   cannot be null

*   defined in: [Create tag category request](tagcategory-definitions-tagcategorytype.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/tags/createTagCategory.json#/properties/categoryType")

### categoryType Type

`string`

### categoryType Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value              | Explanation |
| :----------------- | :---------- |
| `"DESCRIPTIVE"`    |             |
| `"CLASSIFICATION"` |             |
