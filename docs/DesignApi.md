# DesignApi

All URIs are relative to *https://apidevcdn.tweak.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**designCount**](DesignApi.md#designCount) | **GET** /Designs/count | Count instances of the model matched by where from the data source.
[**designCreate**](DesignApi.md#designCreate) | **POST** /Designs | Create a new instance of the model and persist it into the data source.
[**designCreateChangeStreamGetDesignsChangeStream**](DesignApi.md#designCreateChangeStreamGetDesignsChangeStream) | **GET** /Designs/change-stream | Create a change stream.
[**designCreateChangeStreamPostDesignsChangeStream**](DesignApi.md#designCreateChangeStreamPostDesignsChangeStream) | **POST** /Designs/change-stream | Create a change stream.
[**designDeleteById**](DesignApi.md#designDeleteById) | **DELETE** /Designs/{id} | Delete a model instance by {{id}} from the data source.
[**designExistsGetDesignsidExists**](DesignApi.md#designExistsGetDesignsidExists) | **GET** /Designs/{id}/exists | Check whether a model instance exists in the data source.
[**designExistsHeadDesignsid**](DesignApi.md#designExistsHeadDesignsid) | **HEAD** /Designs/{id} | Check whether a model instance exists in the data source.
[**designFind**](DesignApi.md#designFind) | **GET** /Designs | Find all instances of the model matched by filter from the data source.
[**designFindById**](DesignApi.md#designFindById) | **GET** /Designs/{id} | Find a model instance by {{id}} from the data source.
[**designFindOne**](DesignApi.md#designFindOne) | **GET** /Designs/findOne | Find first instance of the model matched by filter from the data source.
[**designPrototypeCountCategories**](DesignApi.md#designPrototypeCountCategories) | **GET** /Designs/{id}/categories/count | Counts categories of Design.
[**designPrototypeCountTags**](DesignApi.md#designPrototypeCountTags) | **GET** /Designs/{id}/tags/count | Counts tags of Design.
[**designPrototypeCreateCategories**](DesignApi.md#designPrototypeCreateCategories) | **POST** /Designs/{id}/categories | Creates a new instance in categories of this model.
[**designPrototypeCreateTags**](DesignApi.md#designPrototypeCreateTags) | **POST** /Designs/{id}/tags | Creates a new instance in tags of this model.
[**designPrototypeDeleteCategories**](DesignApi.md#designPrototypeDeleteCategories) | **DELETE** /Designs/{id}/categories | Deletes all categories of this model.
[**designPrototypeDeleteTags**](DesignApi.md#designPrototypeDeleteTags) | **DELETE** /Designs/{id}/tags | Deletes all tags of this model.
[**designPrototypeDestroyByIdCategories**](DesignApi.md#designPrototypeDestroyByIdCategories) | **DELETE** /Designs/{id}/categories/{fk} | Delete a related item by id for categories.
[**designPrototypeDestroyByIdTags**](DesignApi.md#designPrototypeDestroyByIdTags) | **DELETE** /Designs/{id}/tags/{fk} | Delete a related item by id for tags.
[**designPrototypeFindByIdCategories**](DesignApi.md#designPrototypeFindByIdCategories) | **GET** /Designs/{id}/categories/{fk} | Find a related item by id for categories.
[**designPrototypeFindByIdTags**](DesignApi.md#designPrototypeFindByIdTags) | **GET** /Designs/{id}/tags/{fk} | Find a related item by id for tags.
[**designPrototypeGetCategories**](DesignApi.md#designPrototypeGetCategories) | **GET** /Designs/{id}/categories | Queries categories of Design.
[**designPrototypeGetCustomer**](DesignApi.md#designPrototypeGetCustomer) | **GET** /Designs/{id}/customer | Fetches belongsTo relation customer.
[**designPrototypeGetTags**](DesignApi.md#designPrototypeGetTags) | **GET** /Designs/{id}/tags | Queries tags of Design.
[**designPrototypeUpdateAttributesPatchDesignsid**](DesignApi.md#designPrototypeUpdateAttributesPatchDesignsid) | **PATCH** /Designs/{id} | Patch attributes for a model instance and persist it into the data source.
[**designPrototypeUpdateAttributesPutDesignsid**](DesignApi.md#designPrototypeUpdateAttributesPutDesignsid) | **PUT** /Designs/{id} | Patch attributes for a model instance and persist it into the data source.
[**designPrototypeUpdateByIdCategories**](DesignApi.md#designPrototypeUpdateByIdCategories) | **PUT** /Designs/{id}/categories/{fk} | Update a related item by id for categories.
[**designPrototypeUpdateByIdTags**](DesignApi.md#designPrototypeUpdateByIdTags) | **PUT** /Designs/{id}/tags/{fk} | Update a related item by id for tags.
[**designReplaceById**](DesignApi.md#designReplaceById) | **POST** /Designs/{id}/replace | Replace attributes for a model instance and persist it into the data source.
[**designReplaceOrCreate**](DesignApi.md#designReplaceOrCreate) | **POST** /Designs/replaceOrCreate | Replace an existing model instance or insert a new one into the data source.
[**designUpdateAll**](DesignApi.md#designUpdateAll) | **POST** /Designs/update | Update instances of the model matched by {{where}} from the data source.
[**designUpsertPatchDesigns**](DesignApi.md#designUpsertPatchDesigns) | **PATCH** /Designs | Patch an existing model instance or insert a new one into the data source.
[**designUpsertPutDesigns**](DesignApi.md#designUpsertPutDesigns) | **PUT** /Designs | Patch an existing model instance or insert a new one into the data source.
[**designUpsertWithWhere**](DesignApi.md#designUpsertWithWhere) | **POST** /Designs/upsertWithWhere | Update an existing model instance or insert a new one into the data source based on the where criteria.


<a name="designCount"></a>
# **designCount**
> InlineResponse200 designCount(where)

Count instances of the model matched by where from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String where = "where_example"; // String | Criteria to match model instances
try {
    InlineResponse200 result = apiInstance.designCount(where);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designCount");
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

<a name="designCreate"></a>
# **designCreate**
> Design designCreate(data)

Create a new instance of the model and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
Design data = new Design(); // Design | Model instance data
try {
    Design result = apiInstance.designCreate(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designCreate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Design**](Design.md)| Model instance data | [optional]

### Return type

[**Design**](Design.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designCreateChangeStreamGetDesignsChangeStream"></a>
# **designCreateChangeStreamGetDesignsChangeStream**
> File designCreateChangeStreamGetDesignsChangeStream(options)

Create a change stream.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String options = "options_example"; // String | 
try {
    File result = apiInstance.designCreateChangeStreamGetDesignsChangeStream(options);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designCreateChangeStreamGetDesignsChangeStream");
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

<a name="designCreateChangeStreamPostDesignsChangeStream"></a>
# **designCreateChangeStreamPostDesignsChangeStream**
> File designCreateChangeStreamPostDesignsChangeStream(options)

Create a change stream.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String options = "options_example"; // String | 
try {
    File result = apiInstance.designCreateChangeStreamPostDesignsChangeStream(options);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designCreateChangeStreamPostDesignsChangeStream");
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

<a name="designDeleteById"></a>
# **designDeleteById**
> Object designDeleteById(id)

Delete a model instance by {{id}} from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Model id
try {
    Object result = apiInstance.designDeleteById(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designDeleteById");
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

<a name="designExistsGetDesignsidExists"></a>
# **designExistsGetDesignsidExists**
> InlineResponse2002 designExistsGetDesignsidExists(id)

Check whether a model instance exists in the data source.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Model id
try {
    InlineResponse2002 result = apiInstance.designExistsGetDesignsidExists(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designExistsGetDesignsidExists");
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

<a name="designExistsHeadDesignsid"></a>
# **designExistsHeadDesignsid**
> InlineResponse2002 designExistsHeadDesignsid(id)

Check whether a model instance exists in the data source.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Model id
try {
    InlineResponse2002 result = apiInstance.designExistsHeadDesignsid(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designExistsHeadDesignsid");
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

<a name="designFind"></a>
# **designFind**
> List&lt;Design&gt; designFind(filter)

Find all instances of the model matched by filter from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String filter = "filter_example"; // String | Filter defining fields, where, include, order, offset, and limit
try {
    List<Design> result = apiInstance.designFind(filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designFind");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **String**| Filter defining fields, where, include, order, offset, and limit | [optional]

### Return type

[**List&lt;Design&gt;**](Design.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designFindById"></a>
# **designFindById**
> Design designFindById(id, filter)

Find a model instance by {{id}} from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Model id
String filter = "filter_example"; // String | Filter defining fields and include
try {
    Design result = apiInstance.designFindById(id, filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designFindById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Model id |
 **filter** | **String**| Filter defining fields and include | [optional]

### Return type

[**Design**](Design.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designFindOne"></a>
# **designFindOne**
> Design designFindOne(filter)

Find first instance of the model matched by filter from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String filter = "filter_example"; // String | Filter defining fields, where, include, order, offset, and limit
try {
    Design result = apiInstance.designFindOne(filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designFindOne");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **String**| Filter defining fields, where, include, order, offset, and limit | [optional]

### Return type

[**Design**](Design.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeCountCategories"></a>
# **designPrototypeCountCategories**
> InlineResponse200 designPrototypeCountCategories(id, where)

Counts categories of Design.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
String where = "where_example"; // String | Criteria to match model instances
try {
    InlineResponse200 result = apiInstance.designPrototypeCountCategories(id, where);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeCountCategories");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |
 **where** | **String**| Criteria to match model instances | [optional]

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeCountTags"></a>
# **designPrototypeCountTags**
> InlineResponse200 designPrototypeCountTags(id, where)

Counts tags of Design.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
String where = "where_example"; // String | Criteria to match model instances
try {
    InlineResponse200 result = apiInstance.designPrototypeCountTags(id, where);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeCountTags");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |
 **where** | **String**| Criteria to match model instances | [optional]

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeCreateCategories"></a>
# **designPrototypeCreateCategories**
> Category designPrototypeCreateCategories(id, data)

Creates a new instance in categories of this model.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
Category data = new Category(); // Category | 
try {
    Category result = apiInstance.designPrototypeCreateCategories(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeCreateCategories");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |
 **data** | [**Category**](Category.md)|  | [optional]

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeCreateTags"></a>
# **designPrototypeCreateTags**
> Tag designPrototypeCreateTags(id, data)

Creates a new instance in tags of this model.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
Tag data = new Tag(); // Tag | 
try {
    Tag result = apiInstance.designPrototypeCreateTags(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeCreateTags");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |
 **data** | [**Tag**](Tag.md)|  | [optional]

### Return type

[**Tag**](Tag.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeDeleteCategories"></a>
# **designPrototypeDeleteCategories**
> designPrototypeDeleteCategories(id)

Deletes all categories of this model.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
try {
    apiInstance.designPrototypeDeleteCategories(id);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeDeleteCategories");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |

### Return type

null (empty response body)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeDeleteTags"></a>
# **designPrototypeDeleteTags**
> designPrototypeDeleteTags(id)

Deletes all tags of this model.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
try {
    apiInstance.designPrototypeDeleteTags(id);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeDeleteTags");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |

### Return type

null (empty response body)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeDestroyByIdCategories"></a>
# **designPrototypeDestroyByIdCategories**
> designPrototypeDestroyByIdCategories(id, fk)

Delete a related item by id for categories.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
String fk = "fk_example"; // String | Foreign key for categories
try {
    apiInstance.designPrototypeDestroyByIdCategories(id, fk);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeDestroyByIdCategories");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |
 **fk** | **String**| Foreign key for categories |

### Return type

null (empty response body)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeDestroyByIdTags"></a>
# **designPrototypeDestroyByIdTags**
> designPrototypeDestroyByIdTags(id, fk)

Delete a related item by id for tags.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
String fk = "fk_example"; // String | Foreign key for tags
try {
    apiInstance.designPrototypeDestroyByIdTags(id, fk);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeDestroyByIdTags");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |
 **fk** | **String**| Foreign key for tags |

### Return type

null (empty response body)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeFindByIdCategories"></a>
# **designPrototypeFindByIdCategories**
> Category designPrototypeFindByIdCategories(id, fk)

Find a related item by id for categories.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
String fk = "fk_example"; // String | Foreign key for categories
try {
    Category result = apiInstance.designPrototypeFindByIdCategories(id, fk);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeFindByIdCategories");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |
 **fk** | **String**| Foreign key for categories |

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeFindByIdTags"></a>
# **designPrototypeFindByIdTags**
> Tag designPrototypeFindByIdTags(id, fk)

Find a related item by id for tags.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
String fk = "fk_example"; // String | Foreign key for tags
try {
    Tag result = apiInstance.designPrototypeFindByIdTags(id, fk);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeFindByIdTags");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |
 **fk** | **String**| Foreign key for tags |

### Return type

[**Tag**](Tag.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeGetCategories"></a>
# **designPrototypeGetCategories**
> List&lt;Category&gt; designPrototypeGetCategories(id, filter)

Queries categories of Design.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
String filter = "filter_example"; // String | 
try {
    List<Category> result = apiInstance.designPrototypeGetCategories(id, filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeGetCategories");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |
 **filter** | **String**|  | [optional]

### Return type

[**List&lt;Category&gt;**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeGetCustomer"></a>
# **designPrototypeGetCustomer**
> Customer designPrototypeGetCustomer(id, refresh)

Fetches belongsTo relation customer.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
Boolean refresh = true; // Boolean | 
try {
    Customer result = apiInstance.designPrototypeGetCustomer(id, refresh);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeGetCustomer");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |
 **refresh** | **Boolean**|  | [optional]

### Return type

[**Customer**](Customer.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeGetTags"></a>
# **designPrototypeGetTags**
> List&lt;Tag&gt; designPrototypeGetTags(id, filter)

Queries tags of Design.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
String filter = "filter_example"; // String | 
try {
    List<Tag> result = apiInstance.designPrototypeGetTags(id, filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeGetTags");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |
 **filter** | **String**|  | [optional]

### Return type

[**List&lt;Tag&gt;**](Tag.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeUpdateAttributesPatchDesignsid"></a>
# **designPrototypeUpdateAttributesPatchDesignsid**
> Design designPrototypeUpdateAttributesPatchDesignsid(id, data)

Patch attributes for a model instance and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
Design data = new Design(); // Design | An object of model property name/value pairs
try {
    Design result = apiInstance.designPrototypeUpdateAttributesPatchDesignsid(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeUpdateAttributesPatchDesignsid");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |
 **data** | [**Design**](Design.md)| An object of model property name/value pairs | [optional]

### Return type

[**Design**](Design.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeUpdateAttributesPutDesignsid"></a>
# **designPrototypeUpdateAttributesPutDesignsid**
> Design designPrototypeUpdateAttributesPutDesignsid(id, data)

Patch attributes for a model instance and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
Design data = new Design(); // Design | An object of model property name/value pairs
try {
    Design result = apiInstance.designPrototypeUpdateAttributesPutDesignsid(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeUpdateAttributesPutDesignsid");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |
 **data** | [**Design**](Design.md)| An object of model property name/value pairs | [optional]

### Return type

[**Design**](Design.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeUpdateByIdCategories"></a>
# **designPrototypeUpdateByIdCategories**
> Category designPrototypeUpdateByIdCategories(id, fk, data)

Update a related item by id for categories.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
String fk = "fk_example"; // String | Foreign key for categories
Category data = new Category(); // Category | 
try {
    Category result = apiInstance.designPrototypeUpdateByIdCategories(id, fk, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeUpdateByIdCategories");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |
 **fk** | **String**| Foreign key for categories |
 **data** | [**Category**](Category.md)|  | [optional]

### Return type

[**Category**](Category.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designPrototypeUpdateByIdTags"></a>
# **designPrototypeUpdateByIdTags**
> Tag designPrototypeUpdateByIdTags(id, fk, data)

Update a related item by id for tags.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Design id
String fk = "fk_example"; // String | Foreign key for tags
Tag data = new Tag(); // Tag | 
try {
    Tag result = apiInstance.designPrototypeUpdateByIdTags(id, fk, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designPrototypeUpdateByIdTags");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Design id |
 **fk** | **String**| Foreign key for tags |
 **data** | [**Tag**](Tag.md)|  | [optional]

### Return type

[**Tag**](Tag.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designReplaceById"></a>
# **designReplaceById**
> Design designReplaceById(id, data)

Replace attributes for a model instance and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String id = "id_example"; // String | Model id
Design data = new Design(); // Design | Model instance data
try {
    Design result = apiInstance.designReplaceById(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designReplaceById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Model id |
 **data** | [**Design**](Design.md)| Model instance data | [optional]

### Return type

[**Design**](Design.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designReplaceOrCreate"></a>
# **designReplaceOrCreate**
> Design designReplaceOrCreate(data)

Replace an existing model instance or insert a new one into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
Design data = new Design(); // Design | Model instance data
try {
    Design result = apiInstance.designReplaceOrCreate(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designReplaceOrCreate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Design**](Design.md)| Model instance data | [optional]

### Return type

[**Design**](Design.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designUpdateAll"></a>
# **designUpdateAll**
> InlineResponse2001 designUpdateAll(where, data)

Update instances of the model matched by {{where}} from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String where = "where_example"; // String | Criteria to match model instances
Design data = new Design(); // Design | An object of model property name/value pairs
try {
    InlineResponse2001 result = apiInstance.designUpdateAll(where, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designUpdateAll");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **where** | **String**| Criteria to match model instances | [optional]
 **data** | [**Design**](Design.md)| An object of model property name/value pairs | [optional]

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designUpsertPatchDesigns"></a>
# **designUpsertPatchDesigns**
> Design designUpsertPatchDesigns(data)

Patch an existing model instance or insert a new one into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
Design data = new Design(); // Design | Model instance data
try {
    Design result = apiInstance.designUpsertPatchDesigns(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designUpsertPatchDesigns");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Design**](Design.md)| Model instance data | [optional]

### Return type

[**Design**](Design.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designUpsertPutDesigns"></a>
# **designUpsertPutDesigns**
> Design designUpsertPutDesigns(data)

Patch an existing model instance or insert a new one into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
Design data = new Design(); // Design | Model instance data
try {
    Design result = apiInstance.designUpsertPutDesigns(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designUpsertPutDesigns");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Design**](Design.md)| Model instance data | [optional]

### Return type

[**Design**](Design.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="designUpsertWithWhere"></a>
# **designUpsertWithWhere**
> Design designUpsertWithWhere(where, data)

Update an existing model instance or insert a new one into the data source based on the where criteria.

### Example
```java
// Import classes:
//import com.tweak.api.DesignApi;

DesignApi apiInstance = new DesignApi();
String where = "where_example"; // String | Criteria to match model instances
Design data = new Design(); // Design | An object of model property name/value pairs
try {
    Design result = apiInstance.designUpsertWithWhere(where, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DesignApi#designUpsertWithWhere");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **where** | **String**| Criteria to match model instances | [optional]
 **data** | [**Design**](Design.md)| An object of model property name/value pairs | [optional]

### Return type

[**Design**](Design.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

