# CategoryApi

All URIs are relative to *https://apidevcdn.tweak.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**categoryCount**](CategoryApi.md#categoryCount) | **GET** /Categories/count | Count instances of the model matched by where from the data source.
[**categoryCreate**](CategoryApi.md#categoryCreate) | **POST** /Categories | Create a new instance of the model and persist it into the data source.
[**categoryCreateChangeStreamGetCategoriesChangeStream**](CategoryApi.md#categoryCreateChangeStreamGetCategoriesChangeStream) | **GET** /Categories/change-stream | Create a change stream.
[**categoryCreateChangeStreamPostCategoriesChangeStream**](CategoryApi.md#categoryCreateChangeStreamPostCategoriesChangeStream) | **POST** /Categories/change-stream | Create a change stream.
[**categoryDeleteById**](CategoryApi.md#categoryDeleteById) | **DELETE** /Categories/{id} | Delete a model instance by {{id}} from the data source.
[**categoryExistsGetCategoriesidExists**](CategoryApi.md#categoryExistsGetCategoriesidExists) | **GET** /Categories/{id}/exists | Check whether a model instance exists in the data source.
[**categoryExistsHeadCategoriesid**](CategoryApi.md#categoryExistsHeadCategoriesid) | **HEAD** /Categories/{id} | Check whether a model instance exists in the data source.
[**categoryFind**](CategoryApi.md#categoryFind) | **GET** /Categories | Find all instances of the model matched by filter from the data source.
[**categoryFindById**](CategoryApi.md#categoryFindById) | **GET** /Categories/{id} | Find a model instance by {{id}} from the data source.
[**categoryFindOne**](CategoryApi.md#categoryFindOne) | **GET** /Categories/findOne | Find first instance of the model matched by filter from the data source.
[**categoryPrototypeCountChildren**](CategoryApi.md#categoryPrototypeCountChildren) | **GET** /Categories/{id}/children/count | Counts children of Category.
[**categoryPrototypeCreateChildren**](CategoryApi.md#categoryPrototypeCreateChildren) | **POST** /Categories/{id}/children | Creates a new instance in children of this model.
[**categoryPrototypeDeleteChildren**](CategoryApi.md#categoryPrototypeDeleteChildren) | **DELETE** /Categories/{id}/children | Deletes all children of this model.
[**categoryPrototypeDestroyByIdChildren**](CategoryApi.md#categoryPrototypeDestroyByIdChildren) | **DELETE** /Categories/{id}/children/{fk} | Delete a related item by id for children.
[**categoryPrototypeFindByIdChildren**](CategoryApi.md#categoryPrototypeFindByIdChildren) | **GET** /Categories/{id}/children/{fk} | Find a related item by id for children.
[**categoryPrototypeGetChildren**](CategoryApi.md#categoryPrototypeGetChildren) | **GET** /Categories/{id}/children | Queries children of Category.
[**categoryPrototypeGetParent**](CategoryApi.md#categoryPrototypeGetParent) | **GET** /Categories/{id}/parent | Fetches belongsTo relation parent.
[**categoryPrototypeUpdateAttributesPatchCategoriesid**](CategoryApi.md#categoryPrototypeUpdateAttributesPatchCategoriesid) | **PATCH** /Categories/{id} | Patch attributes for a model instance and persist it into the data source.
[**categoryPrototypeUpdateAttributesPutCategoriesid**](CategoryApi.md#categoryPrototypeUpdateAttributesPutCategoriesid) | **PUT** /Categories/{id} | Patch attributes for a model instance and persist it into the data source.
[**categoryPrototypeUpdateByIdChildren**](CategoryApi.md#categoryPrototypeUpdateByIdChildren) | **PUT** /Categories/{id}/children/{fk} | Update a related item by id for children.
[**categoryReplaceById**](CategoryApi.md#categoryReplaceById) | **POST** /Categories/{id}/replace | Replace attributes for a model instance and persist it into the data source.
[**categoryReplaceOrCreate**](CategoryApi.md#categoryReplaceOrCreate) | **POST** /Categories/replaceOrCreate | Replace an existing model instance or insert a new one into the data source.
[**categoryUpdateAll**](CategoryApi.md#categoryUpdateAll) | **POST** /Categories/update | Update instances of the model matched by {{where}} from the data source.
[**categoryUpsertPatchCategories**](CategoryApi.md#categoryUpsertPatchCategories) | **PATCH** /Categories | Patch an existing model instance or insert a new one into the data source.
[**categoryUpsertPutCategories**](CategoryApi.md#categoryUpsertPutCategories) | **PUT** /Categories | Patch an existing model instance or insert a new one into the data source.
[**categoryUpsertWithWhere**](CategoryApi.md#categoryUpsertWithWhere) | **POST** /Categories/upsertWithWhere | Update an existing model instance or insert a new one into the data source based on the where criteria.


<a name="categoryCount"></a>
# **categoryCount**
> InlineResponse200 categoryCount(where)

Count instances of the model matched by where from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String where = "where_example"; // String | Criteria to match model instances
try {
    InlineResponse200 result = apiInstance.categoryCount(where);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryCount");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **where** | **String**| Criteria to match model instances | [optional]

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryCreate"></a>
# **categoryCreate**
> Category categoryCreate(data)

Create a new instance of the model and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
Category data = new Category(); // Category | Model instance data
try {
    Category result = apiInstance.categoryCreate(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryCreate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Category**](Category.md)| Model instance data | [optional]

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryCreateChangeStreamGetCategoriesChangeStream"></a>
# **categoryCreateChangeStreamGetCategoriesChangeStream**
> File categoryCreateChangeStreamGetCategoriesChangeStream(options)

Create a change stream.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String options = "options_example"; // String | 
try {
    File result = apiInstance.categoryCreateChangeStreamGetCategoriesChangeStream(options);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryCreateChangeStreamGetCategoriesChangeStream");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **options** | **String**|  | [optional]

### Return type

[**File**](File.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryCreateChangeStreamPostCategoriesChangeStream"></a>
# **categoryCreateChangeStreamPostCategoriesChangeStream**
> File categoryCreateChangeStreamPostCategoriesChangeStream(options)

Create a change stream.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String options = "options_example"; // String | 
try {
    File result = apiInstance.categoryCreateChangeStreamPostCategoriesChangeStream(options);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryCreateChangeStreamPostCategoriesChangeStream");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **options** | **String**|  | [optional]

### Return type

[**File**](File.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryDeleteById"></a>
# **categoryDeleteById**
> Object categoryDeleteById(id)

Delete a model instance by {{id}} from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String id = "id_example"; // String | Model id
try {
    Object result = apiInstance.categoryDeleteById(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryDeleteById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Model id |

### Return type

**Object**

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryExistsGetCategoriesidExists"></a>
# **categoryExistsGetCategoriesidExists**
> InlineResponse2002 categoryExistsGetCategoriesidExists(id)

Check whether a model instance exists in the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String id = "id_example"; // String | Model id
try {
    InlineResponse2002 result = apiInstance.categoryExistsGetCategoriesidExists(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryExistsGetCategoriesidExists");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Model id |

### Return type

[**InlineResponse2002**](InlineResponse2002.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryExistsHeadCategoriesid"></a>
# **categoryExistsHeadCategoriesid**
> InlineResponse2002 categoryExistsHeadCategoriesid(id)

Check whether a model instance exists in the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String id = "id_example"; // String | Model id
try {
    InlineResponse2002 result = apiInstance.categoryExistsHeadCategoriesid(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryExistsHeadCategoriesid");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Model id |

### Return type

[**InlineResponse2002**](InlineResponse2002.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryFind"></a>
# **categoryFind**
> List&lt;Category&gt; categoryFind(filter)

Find all instances of the model matched by filter from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String filter = "filter_example"; // String | Filter defining fields, where, include, order, offset, and limit
try {
    List<Category> result = apiInstance.categoryFind(filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryFind");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **String**| Filter defining fields, where, include, order, offset, and limit | [optional]

### Return type

[**List&lt;Category&gt;**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryFindById"></a>
# **categoryFindById**
> Category categoryFindById(id, filter)

Find a model instance by {{id}} from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String id = "id_example"; // String | Model id
String filter = "filter_example"; // String | Filter defining fields and include
try {
    Category result = apiInstance.categoryFindById(id, filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryFindById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Model id |
 **filter** | **String**| Filter defining fields and include | [optional]

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryFindOne"></a>
# **categoryFindOne**
> Category categoryFindOne(filter)

Find first instance of the model matched by filter from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String filter = "filter_example"; // String | Filter defining fields, where, include, order, offset, and limit
try {
    Category result = apiInstance.categoryFindOne(filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryFindOne");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **String**| Filter defining fields, where, include, order, offset, and limit | [optional]

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryPrototypeCountChildren"></a>
# **categoryPrototypeCountChildren**
> InlineResponse200 categoryPrototypeCountChildren(id, where)

Counts children of Category.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String id = "id_example"; // String | Category id
String where = "where_example"; // String | Criteria to match model instances
try {
    InlineResponse200 result = apiInstance.categoryPrototypeCountChildren(id, where);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryPrototypeCountChildren");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Category id |
 **where** | **String**| Criteria to match model instances | [optional]

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryPrototypeCreateChildren"></a>
# **categoryPrototypeCreateChildren**
> Category categoryPrototypeCreateChildren(id, data)

Creates a new instance in children of this model.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String id = "id_example"; // String | Category id
Category data = new Category(); // Category | 
try {
    Category result = apiInstance.categoryPrototypeCreateChildren(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryPrototypeCreateChildren");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Category id |
 **data** | [**Category**](Category.md)|  | [optional]

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryPrototypeDeleteChildren"></a>
# **categoryPrototypeDeleteChildren**
> categoryPrototypeDeleteChildren(id)

Deletes all children of this model.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String id = "id_example"; // String | Category id
try {
    apiInstance.categoryPrototypeDeleteChildren(id);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryPrototypeDeleteChildren");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Category id |

### Return type

null (empty response body)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryPrototypeDestroyByIdChildren"></a>
# **categoryPrototypeDestroyByIdChildren**
> categoryPrototypeDestroyByIdChildren(id, fk)

Delete a related item by id for children.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String id = "id_example"; // String | Category id
String fk = "fk_example"; // String | Foreign key for children
try {
    apiInstance.categoryPrototypeDestroyByIdChildren(id, fk);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryPrototypeDestroyByIdChildren");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Category id |
 **fk** | **String**| Foreign key for children |

### Return type

null (empty response body)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryPrototypeFindByIdChildren"></a>
# **categoryPrototypeFindByIdChildren**
> Category categoryPrototypeFindByIdChildren(id, fk)

Find a related item by id for children.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String id = "id_example"; // String | Category id
String fk = "fk_example"; // String | Foreign key for children
try {
    Category result = apiInstance.categoryPrototypeFindByIdChildren(id, fk);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryPrototypeFindByIdChildren");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Category id |
 **fk** | **String**| Foreign key for children |

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryPrototypeGetChildren"></a>
# **categoryPrototypeGetChildren**
> List&lt;Category&gt; categoryPrototypeGetChildren(id, filter)

Queries children of Category.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String id = "id_example"; // String | Category id
String filter = "filter_example"; // String | 
try {
    List<Category> result = apiInstance.categoryPrototypeGetChildren(id, filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryPrototypeGetChildren");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Category id |
 **filter** | **String**|  | [optional]

### Return type

[**List&lt;Category&gt;**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryPrototypeGetParent"></a>
# **categoryPrototypeGetParent**
> Category categoryPrototypeGetParent(id, refresh)

Fetches belongsTo relation parent.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String id = "id_example"; // String | Category id
Boolean refresh = true; // Boolean | 
try {
    Category result = apiInstance.categoryPrototypeGetParent(id, refresh);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryPrototypeGetParent");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Category id |
 **refresh** | **Boolean**|  | [optional]

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryPrototypeUpdateAttributesPatchCategoriesid"></a>
# **categoryPrototypeUpdateAttributesPatchCategoriesid**
> Category categoryPrototypeUpdateAttributesPatchCategoriesid(id, data)

Patch attributes for a model instance and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String id = "id_example"; // String | Category id
Category data = new Category(); // Category | An object of model property name/value pairs
try {
    Category result = apiInstance.categoryPrototypeUpdateAttributesPatchCategoriesid(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryPrototypeUpdateAttributesPatchCategoriesid");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Category id |
 **data** | [**Category**](Category.md)| An object of model property name/value pairs | [optional]

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryPrototypeUpdateAttributesPutCategoriesid"></a>
# **categoryPrototypeUpdateAttributesPutCategoriesid**
> Category categoryPrototypeUpdateAttributesPutCategoriesid(id, data)

Patch attributes for a model instance and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String id = "id_example"; // String | Category id
Category data = new Category(); // Category | An object of model property name/value pairs
try {
    Category result = apiInstance.categoryPrototypeUpdateAttributesPutCategoriesid(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryPrototypeUpdateAttributesPutCategoriesid");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Category id |
 **data** | [**Category**](Category.md)| An object of model property name/value pairs | [optional]

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryPrototypeUpdateByIdChildren"></a>
# **categoryPrototypeUpdateByIdChildren**
> Category categoryPrototypeUpdateByIdChildren(id, fk, data)

Update a related item by id for children.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String id = "id_example"; // String | Category id
String fk = "fk_example"; // String | Foreign key for children
Category data = new Category(); // Category | 
try {
    Category result = apiInstance.categoryPrototypeUpdateByIdChildren(id, fk, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryPrototypeUpdateByIdChildren");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Category id |
 **fk** | **String**| Foreign key for children |
 **data** | [**Category**](Category.md)|  | [optional]

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryReplaceById"></a>
# **categoryReplaceById**
> Category categoryReplaceById(id, data)

Replace attributes for a model instance and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String id = "id_example"; // String | Model id
Category data = new Category(); // Category | Model instance data
try {
    Category result = apiInstance.categoryReplaceById(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryReplaceById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Model id |
 **data** | [**Category**](Category.md)| Model instance data | [optional]

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryReplaceOrCreate"></a>
# **categoryReplaceOrCreate**
> Category categoryReplaceOrCreate(data)

Replace an existing model instance or insert a new one into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
Category data = new Category(); // Category | Model instance data
try {
    Category result = apiInstance.categoryReplaceOrCreate(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryReplaceOrCreate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Category**](Category.md)| Model instance data | [optional]

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryUpdateAll"></a>
# **categoryUpdateAll**
> InlineResponse2001 categoryUpdateAll(where, data)

Update instances of the model matched by {{where}} from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String where = "where_example"; // String | Criteria to match model instances
Category data = new Category(); // Category | An object of model property name/value pairs
try {
    InlineResponse2001 result = apiInstance.categoryUpdateAll(where, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryUpdateAll");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **where** | **String**| Criteria to match model instances | [optional]
 **data** | [**Category**](Category.md)| An object of model property name/value pairs | [optional]

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryUpsertPatchCategories"></a>
# **categoryUpsertPatchCategories**
> Category categoryUpsertPatchCategories(data)

Patch an existing model instance or insert a new one into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
Category data = new Category(); // Category | Model instance data
try {
    Category result = apiInstance.categoryUpsertPatchCategories(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryUpsertPatchCategories");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Category**](Category.md)| Model instance data | [optional]

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryUpsertPutCategories"></a>
# **categoryUpsertPutCategories**
> Category categoryUpsertPutCategories(data)

Patch an existing model instance or insert a new one into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
Category data = new Category(); // Category | Model instance data
try {
    Category result = apiInstance.categoryUpsertPutCategories(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryUpsertPutCategories");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Category**](Category.md)| Model instance data | [optional]

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="categoryUpsertWithWhere"></a>
# **categoryUpsertWithWhere**
> Category categoryUpsertWithWhere(where, data)

Update an existing model instance or insert a new one into the data source based on the where criteria.

### Example
```java
// Import classes:
//import com.tweak.api.CategoryApi;

CategoryApi apiInstance = new CategoryApi();
String where = "where_example"; // String | Criteria to match model instances
Category data = new Category(); // Category | An object of model property name/value pairs
try {
    Category result = apiInstance.categoryUpsertWithWhere(where, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CategoryApi#categoryUpsertWithWhere");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **where** | **String**| Criteria to match model instances | [optional]
 **data** | [**Category**](Category.md)| An object of model property name/value pairs | [optional]

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

