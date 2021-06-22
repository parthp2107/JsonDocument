# Create tag API request Schema

```txt
https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/tags/createTag.json
```

Create tag API request

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                              |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [createTag.json](../out/api/tags/createTag.json "open original schema") |

## Create tag API request Type

`object` ([Create tag API request](createtag.md))

# Create tag API request Properties

| Property                    | Type     | Required | Nullable       | Defined by                                                                                                                                                                                                                |
| :-------------------------- | :------- | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [name](#name)               | `string` | Required | cannot be null | [Create tag API request](tagcategory-definitions-tagname.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/tags/createTag.json#/properties/name")         |
| [description](#description) | `string` | Required | cannot be null | [Create tag API request](createtag-properties-description.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/tags/createTag.json#/properties/description") |
| [tags](#tags)               | `array`  | Optional | cannot be null | [Create tag API request](createtag-properties-tags.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/tags/createTag.json#/properties/tags")               |

## name

Name of the tag

`name`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Create tag API request](tagcategory-definitions-tagname.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/tags/createTag.json#/properties/name")

### name Type

`string`

### name Constraints

**maximum length**: the maximum number of characters for this string is: `25`

**minimum length**: the minimum number of characters for this string is: `2`

## description

Unique name of the tag category

`description`

*   is required

*   Type: `string`

*   cannot be null

*   defined in: [Create tag API request](createtag-properties-description.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/tags/createTag.json#/properties/description")

### description Type

`string`

## tags

Fully qualified names of tags associated with this tag

`tags`

*   is optional

*   Type: `string[]`

*   cannot be null

*   defined in: [Create tag API request](createtag-properties-tags.md "https://github.com/StreamlineData/catalog/blob/master/catalog-rest-service/src/main/resources/json/schema/api/tags/createTag.json#/properties/tags")

### tags Type

`string[]`
