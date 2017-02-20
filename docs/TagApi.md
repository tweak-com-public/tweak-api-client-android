# TagApi

All URIs are relative to *https://apidevcdn.tweak.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**tagCount**](TagApi.md#tagCount) | **GET** /Tags/count | Count instances of the model matched by where from the data source.
[**tagCreate**](TagApi.md#tagCreate) | **POST** /Tags | Create a new instance of the model and persist it into the data source.
[**tagCreateChangeStreamGetTagsChangeStream**](TagApi.md#tagCreateChangeStreamGetTagsChangeStream) | **GET** /Tags/change-stream | Create a change stream.
[**tagCreateChangeStreamPostTagsChangeStream**](TagApi.md#tagCreateChangeStreamPostTagsChangeStream) | **POST** /Tags/change-stream | Create a change stream.
[**tagDeleteById**](TagApi.md#tagDeleteById) | **DELETE** /Tags/{id} | Delete a model instance by {{id}} from the data source.
[**tagExistsGetTagsidExists**](TagApi.md#tagExistsGetTagsidExists) | **GET** /Tags/{id}/exists | Check whether a model instance exists in the data source.
[**tagExistsHeadTagsid**](TagApi.md#tagExistsHeadTagsid) | **HEAD** /Tags/{id} | Check whether a model instance exists in the data source.
[**tagFind**](TagApi.md#tagFind) | **GET** /Tags | Find all instances of the model matched by filter from the data source.
[**tagFindById**](TagApi.md#tagFindById) | **GET** /Tags/{id} | Find a model instance by {{id}} from the data source.
[**tagFindOne**](TagApi.md#tagFindOne) | **GET** /Tags/findOne | Find first instance of the model matched by filter from the data source.
[**tagPrototypeUpdateAttributesPatchTagsid**](TagApi.md#tagPrototypeUpdateAttributesPatchTagsid) | **PATCH** /Tags/{id} | Patch attributes for a model instance and persist it into the data source.
[**tagPrototypeUpdateAttributesPutTagsid**](TagApi.md#tagPrototypeUpdateAttributesPutTagsid) | **PUT** /Tags/{id} | Patch attributes for a model instance and persist it into the data source.
[**tagReplaceById**](TagApi.md#tagReplaceById) | **POST** /Tags/{id}/replace | Replace attributes for a model instance and persist it into the data source.
[**tagReplaceOrCreate**](TagApi.md#tagReplaceOrCreate) | **POST** /Tags/replaceOrCreate | Replace an existing model instance or insert a new one into the data source.
[**tagUpdateAll**](TagApi.md#tagUpdateAll) | **POST** /Tags/update | Update instances of the model matched by {{where}} from the data source.
[**tagUpsertPatchTags**](TagApi.md#tagUpsertPatchTags) | **PATCH** /Tags | Patch an existing model instance or insert a new one into the data source.
[**tagUpsertPutTags**](TagApi.md#tagUpsertPutTags) | **PUT** /Tags | Patch an existing model instance or insert a new one into the data source.
[**tagUpsertWithWhere**](TagApi.md#tagUpsertWithWhere) | **POST** /Tags/upsertWithWhere | Update an existing model instance or insert a new one into the data source based on the where criteria.


<a name="tagCount"></a>
# **tagCount**
> InlineResponse200 tagCount(where)

Count instances of the model matched by where from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
String where = "where_example"; // String | Criteria to match model instances
try {
    InlineResponse200 result = apiInstance.tagCount(where);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagCount");
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

<a name="tagCreate"></a>
# **tagCreate**
> Tag tagCreate(data)

Create a new instance of the model and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
Tag data = new Tag(); // Tag | Model instance data
try {
    Tag result = apiInstance.tagCreate(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagCreate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Tag**](Tag.md)| Model instance data | [optional]

### Return type

[**Tag**](Tag.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="tagCreateChangeStreamGetTagsChangeStream"></a>
# **tagCreateChangeStreamGetTagsChangeStream**
> File tagCreateChangeStreamGetTagsChangeStream(options)

Create a change stream.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
String options = "options_example"; // String | 
try {
    File result = apiInstance.tagCreateChangeStreamGetTagsChangeStream(options);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagCreateChangeStreamGetTagsChangeStream");
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

<a name="tagCreateChangeStreamPostTagsChangeStream"></a>
# **tagCreateChangeStreamPostTagsChangeStream**
> File tagCreateChangeStreamPostTagsChangeStream(options)

Create a change stream.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
String options = "options_example"; // String | 
try {
    File result = apiInstance.tagCreateChangeStreamPostTagsChangeStream(options);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagCreateChangeStreamPostTagsChangeStream");
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

<a name="tagDeleteById"></a>
# **tagDeleteById**
> Object tagDeleteById(id)

Delete a model instance by {{id}} from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
String id = "id_example"; // String | Model id
try {
    Object result = apiInstance.tagDeleteById(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagDeleteById");
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

<a name="tagExistsGetTagsidExists"></a>
# **tagExistsGetTagsidExists**
> InlineResponse2002 tagExistsGetTagsidExists(id)

Check whether a model instance exists in the data source.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
String id = "id_example"; // String | Model id
try {
    InlineResponse2002 result = apiInstance.tagExistsGetTagsidExists(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagExistsGetTagsidExists");
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

<a name="tagExistsHeadTagsid"></a>
# **tagExistsHeadTagsid**
> InlineResponse2002 tagExistsHeadTagsid(id)

Check whether a model instance exists in the data source.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
String id = "id_example"; // String | Model id
try {
    InlineResponse2002 result = apiInstance.tagExistsHeadTagsid(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagExistsHeadTagsid");
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

<a name="tagFind"></a>
# **tagFind**
> List&lt;Tag&gt; tagFind(filter)

Find all instances of the model matched by filter from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
String filter = "filter_example"; // String | Filter defining fields, where, include, order, offset, and limit
try {
    List<Tag> result = apiInstance.tagFind(filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagFind");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **String**| Filter defining fields, where, include, order, offset, and limit | [optional]

### Return type

[**List&lt;Tag&gt;**](Tag.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="tagFindById"></a>
# **tagFindById**
> Tag tagFindById(id, filter)

Find a model instance by {{id}} from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
String id = "id_example"; // String | Model id
String filter = "filter_example"; // String | Filter defining fields and include
try {
    Tag result = apiInstance.tagFindById(id, filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagFindById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Model id |
 **filter** | **String**| Filter defining fields and include | [optional]

### Return type

[**Tag**](Tag.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="tagFindOne"></a>
# **tagFindOne**
> Tag tagFindOne(filter)

Find first instance of the model matched by filter from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
String filter = "filter_example"; // String | Filter defining fields, where, include, order, offset, and limit
try {
    Tag result = apiInstance.tagFindOne(filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagFindOne");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **String**| Filter defining fields, where, include, order, offset, and limit | [optional]

### Return type

[**Tag**](Tag.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="tagPrototypeUpdateAttributesPatchTagsid"></a>
# **tagPrototypeUpdateAttributesPatchTagsid**
> Tag tagPrototypeUpdateAttributesPatchTagsid(id, data)

Patch attributes for a model instance and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
String id = "id_example"; // String | Tag id
Tag data = new Tag(); // Tag | An object of model property name/value pairs
try {
    Tag result = apiInstance.tagPrototypeUpdateAttributesPatchTagsid(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagPrototypeUpdateAttributesPatchTagsid");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Tag id |
 **data** | [**Tag**](Tag.md)| An object of model property name/value pairs | [optional]

### Return type

[**Tag**](Tag.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="tagPrototypeUpdateAttributesPutTagsid"></a>
# **tagPrototypeUpdateAttributesPutTagsid**
> Tag tagPrototypeUpdateAttributesPutTagsid(id, data)

Patch attributes for a model instance and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
String id = "id_example"; // String | Tag id
Tag data = new Tag(); // Tag | An object of model property name/value pairs
try {
    Tag result = apiInstance.tagPrototypeUpdateAttributesPutTagsid(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagPrototypeUpdateAttributesPutTagsid");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Tag id |
 **data** | [**Tag**](Tag.md)| An object of model property name/value pairs | [optional]

### Return type

[**Tag**](Tag.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="tagReplaceById"></a>
# **tagReplaceById**
> Tag tagReplaceById(id, data)

Replace attributes for a model instance and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
String id = "id_example"; // String | Model id
Tag data = new Tag(); // Tag | Model instance data
try {
    Tag result = apiInstance.tagReplaceById(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagReplaceById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Model id |
 **data** | [**Tag**](Tag.md)| Model instance data | [optional]

### Return type

[**Tag**](Tag.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="tagReplaceOrCreate"></a>
# **tagReplaceOrCreate**
> Tag tagReplaceOrCreate(data)

Replace an existing model instance or insert a new one into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
Tag data = new Tag(); // Tag | Model instance data
try {
    Tag result = apiInstance.tagReplaceOrCreate(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagReplaceOrCreate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Tag**](Tag.md)| Model instance data | [optional]

### Return type

[**Tag**](Tag.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="tagUpdateAll"></a>
# **tagUpdateAll**
> InlineResponse2001 tagUpdateAll(where, data)

Update instances of the model matched by {{where}} from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
String where = "where_example"; // String | Criteria to match model instances
Tag data = new Tag(); // Tag | An object of model property name/value pairs
try {
    InlineResponse2001 result = apiInstance.tagUpdateAll(where, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagUpdateAll");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **where** | **String**| Criteria to match model instances | [optional]
 **data** | [**Tag**](Tag.md)| An object of model property name/value pairs | [optional]

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="tagUpsertPatchTags"></a>
# **tagUpsertPatchTags**
> Tag tagUpsertPatchTags(data)

Patch an existing model instance or insert a new one into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
Tag data = new Tag(); // Tag | Model instance data
try {
    Tag result = apiInstance.tagUpsertPatchTags(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagUpsertPatchTags");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Tag**](Tag.md)| Model instance data | [optional]

### Return type

[**Tag**](Tag.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="tagUpsertPutTags"></a>
# **tagUpsertPutTags**
> Tag tagUpsertPutTags(data)

Patch an existing model instance or insert a new one into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
Tag data = new Tag(); // Tag | Model instance data
try {
    Tag result = apiInstance.tagUpsertPutTags(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagUpsertPutTags");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Tag**](Tag.md)| Model instance data | [optional]

### Return type

[**Tag**](Tag.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="tagUpsertWithWhere"></a>
# **tagUpsertWithWhere**
> Tag tagUpsertWithWhere(where, data)

Update an existing model instance or insert a new one into the data source based on the where criteria.

### Example
```java
// Import classes:
//import com.tweak.api.TagApi;

TagApi apiInstance = new TagApi();
String where = "where_example"; // String | Criteria to match model instances
Tag data = new Tag(); // Tag | An object of model property name/value pairs
try {
    Tag result = apiInstance.tagUpsertWithWhere(where, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TagApi#tagUpsertWithWhere");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **where** | **String**| Criteria to match model instances | [optional]
 **data** | [**Tag**](Tag.md)| An object of model property name/value pairs | [optional]

### Return type

[**Tag**](Tag.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

