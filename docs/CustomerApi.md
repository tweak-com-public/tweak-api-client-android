# CustomerApi

All URIs are relative to *https://apidevcdn.tweak.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**customerConfirm**](CustomerApi.md#customerConfirm) | **GET** /Customers/confirm | Confirm a user registration with email verification token.
[**customerCount**](CustomerApi.md#customerCount) | **GET** /Customers/count | Count instances of the model matched by where from the data source.
[**customerCreate**](CustomerApi.md#customerCreate) | **POST** /Customers | Create a new instance of the model and persist it into the data source.
[**customerCreateChangeStreamGetCustomersChangeStream**](CustomerApi.md#customerCreateChangeStreamGetCustomersChangeStream) | **GET** /Customers/change-stream | Create a change stream.
[**customerCreateChangeStreamPostCustomersChangeStream**](CustomerApi.md#customerCreateChangeStreamPostCustomersChangeStream) | **POST** /Customers/change-stream | Create a change stream.
[**customerDeleteById**](CustomerApi.md#customerDeleteById) | **DELETE** /Customers/{id} | Delete a model instance by {{id}} from the data source.
[**customerExistsGetCustomersidExists**](CustomerApi.md#customerExistsGetCustomersidExists) | **GET** /Customers/{id}/exists | Check whether a model instance exists in the data source.
[**customerExistsHeadCustomersid**](CustomerApi.md#customerExistsHeadCustomersid) | **HEAD** /Customers/{id} | Check whether a model instance exists in the data source.
[**customerFind**](CustomerApi.md#customerFind) | **GET** /Customers | Find all instances of the model matched by filter from the data source.
[**customerFindById**](CustomerApi.md#customerFindById) | **GET** /Customers/{id} | Find a model instance by {{id}} from the data source.
[**customerFindOne**](CustomerApi.md#customerFindOne) | **GET** /Customers/findOne | Find first instance of the model matched by filter from the data source.
[**customerLogin**](CustomerApi.md#customerLogin) | **POST** /Customers/login | Login a user with username/email and password.
[**customerLogout**](CustomerApi.md#customerLogout) | **POST** /Customers/logout | Logout a user with access token.
[**customerPrototypeCountAccessTokens**](CustomerApi.md#customerPrototypeCountAccessTokens) | **GET** /Customers/{id}/accessTokens/count | Counts accessTokens of Customer.
[**customerPrototypeCountDesigns**](CustomerApi.md#customerPrototypeCountDesigns) | **GET** /Customers/{id}/designs/count | Counts designs of Customer.
[**customerPrototypeCreateAccessTokens**](CustomerApi.md#customerPrototypeCreateAccessTokens) | **POST** /Customers/{id}/accessTokens | Creates a new instance in accessTokens of this model.
[**customerPrototypeCreateDesigns**](CustomerApi.md#customerPrototypeCreateDesigns) | **POST** /Customers/{id}/designs | Creates a new instance in designs of this model.
[**customerPrototypeDeleteAccessTokens**](CustomerApi.md#customerPrototypeDeleteAccessTokens) | **DELETE** /Customers/{id}/accessTokens | Deletes all accessTokens of this model.
[**customerPrototypeDeleteDesigns**](CustomerApi.md#customerPrototypeDeleteDesigns) | **DELETE** /Customers/{id}/designs | Deletes all designs of this model.
[**customerPrototypeDestroyByIdAccessTokens**](CustomerApi.md#customerPrototypeDestroyByIdAccessTokens) | **DELETE** /Customers/{id}/accessTokens/{fk} | Delete a related item by id for accessTokens.
[**customerPrototypeDestroyByIdDesigns**](CustomerApi.md#customerPrototypeDestroyByIdDesigns) | **DELETE** /Customers/{id}/designs/{fk} | Delete a related item by id for designs.
[**customerPrototypeFindByIdAccessTokens**](CustomerApi.md#customerPrototypeFindByIdAccessTokens) | **GET** /Customers/{id}/accessTokens/{fk} | Find a related item by id for accessTokens.
[**customerPrototypeFindByIdDesigns**](CustomerApi.md#customerPrototypeFindByIdDesigns) | **GET** /Customers/{id}/designs/{fk} | Find a related item by id for designs.
[**customerPrototypeGetAccessTokens**](CustomerApi.md#customerPrototypeGetAccessTokens) | **GET** /Customers/{id}/accessTokens | Queries accessTokens of Customer.
[**customerPrototypeGetDesigns**](CustomerApi.md#customerPrototypeGetDesigns) | **GET** /Customers/{id}/designs | Queries designs of Customer.
[**customerPrototypeUpdateAttributesPatchCustomersid**](CustomerApi.md#customerPrototypeUpdateAttributesPatchCustomersid) | **PATCH** /Customers/{id} | Patch attributes for a model instance and persist it into the data source.
[**customerPrototypeUpdateAttributesPutCustomersid**](CustomerApi.md#customerPrototypeUpdateAttributesPutCustomersid) | **PUT** /Customers/{id} | Patch attributes for a model instance and persist it into the data source.
[**customerPrototypeUpdateByIdAccessTokens**](CustomerApi.md#customerPrototypeUpdateByIdAccessTokens) | **PUT** /Customers/{id}/accessTokens/{fk} | Update a related item by id for accessTokens.
[**customerPrototypeUpdateByIdDesigns**](CustomerApi.md#customerPrototypeUpdateByIdDesigns) | **PUT** /Customers/{id}/designs/{fk} | Update a related item by id for designs.
[**customerReplaceById**](CustomerApi.md#customerReplaceById) | **POST** /Customers/{id}/replace | Replace attributes for a model instance and persist it into the data source.
[**customerReplaceOrCreate**](CustomerApi.md#customerReplaceOrCreate) | **POST** /Customers/replaceOrCreate | Replace an existing model instance or insert a new one into the data source.
[**customerResetPassword**](CustomerApi.md#customerResetPassword) | **POST** /Customers/reset | Reset password for a user with email.
[**customerUpdateAll**](CustomerApi.md#customerUpdateAll) | **POST** /Customers/update | Update instances of the model matched by {{where}} from the data source.
[**customerUpsertPatchCustomers**](CustomerApi.md#customerUpsertPatchCustomers) | **PATCH** /Customers | Patch an existing model instance or insert a new one into the data source.
[**customerUpsertPutCustomers**](CustomerApi.md#customerUpsertPutCustomers) | **PUT** /Customers | Patch an existing model instance or insert a new one into the data source.
[**customerUpsertWithWhere**](CustomerApi.md#customerUpsertWithWhere) | **POST** /Customers/upsertWithWhere | Update an existing model instance or insert a new one into the data source based on the where criteria.


<a name="customerConfirm"></a>
# **customerConfirm**
> customerConfirm(uid, token, redirect)

Confirm a user registration with email verification token.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String uid = "uid_example"; // String | 
String token = "token_example"; // String | 
String redirect = "redirect_example"; // String | 
try {
    apiInstance.customerConfirm(uid, token, redirect);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerConfirm");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uid** | **String**|  |
 **token** | **String**|  |
 **redirect** | **String**|  | [optional]

### Return type

null (empty response body)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerCount"></a>
# **customerCount**
> InlineResponse200 customerCount(where)

Count instances of the model matched by where from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String where = "where_example"; // String | Criteria to match model instances
try {
    InlineResponse200 result = apiInstance.customerCount(where);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerCount");
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

<a name="customerCreate"></a>
# **customerCreate**
> Customer customerCreate(data)

Create a new instance of the model and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
Customer data = new Customer(); // Customer | Model instance data
try {
    Customer result = apiInstance.customerCreate(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerCreate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Customer**](Customer.md)| Model instance data | [optional]

### Return type

[**Customer**](Customer.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerCreateChangeStreamGetCustomersChangeStream"></a>
# **customerCreateChangeStreamGetCustomersChangeStream**
> File customerCreateChangeStreamGetCustomersChangeStream(options)

Create a change stream.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String options = "options_example"; // String | 
try {
    File result = apiInstance.customerCreateChangeStreamGetCustomersChangeStream(options);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerCreateChangeStreamGetCustomersChangeStream");
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

<a name="customerCreateChangeStreamPostCustomersChangeStream"></a>
# **customerCreateChangeStreamPostCustomersChangeStream**
> File customerCreateChangeStreamPostCustomersChangeStream(options)

Create a change stream.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String options = "options_example"; // String | 
try {
    File result = apiInstance.customerCreateChangeStreamPostCustomersChangeStream(options);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerCreateChangeStreamPostCustomersChangeStream");
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

<a name="customerDeleteById"></a>
# **customerDeleteById**
> Object customerDeleteById(id)

Delete a model instance by {{id}} from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Model id
try {
    Object result = apiInstance.customerDeleteById(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerDeleteById");
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

<a name="customerExistsGetCustomersidExists"></a>
# **customerExistsGetCustomersidExists**
> InlineResponse2002 customerExistsGetCustomersidExists(id)

Check whether a model instance exists in the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Model id
try {
    InlineResponse2002 result = apiInstance.customerExistsGetCustomersidExists(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerExistsGetCustomersidExists");
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

<a name="customerExistsHeadCustomersid"></a>
# **customerExistsHeadCustomersid**
> InlineResponse2002 customerExistsHeadCustomersid(id)

Check whether a model instance exists in the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Model id
try {
    InlineResponse2002 result = apiInstance.customerExistsHeadCustomersid(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerExistsHeadCustomersid");
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

<a name="customerFind"></a>
# **customerFind**
> List&lt;Customer&gt; customerFind(filter)

Find all instances of the model matched by filter from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String filter = "filter_example"; // String | Filter defining fields, where, include, order, offset, and limit
try {
    List<Customer> result = apiInstance.customerFind(filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerFind");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **String**| Filter defining fields, where, include, order, offset, and limit | [optional]

### Return type

[**List&lt;Customer&gt;**](Customer.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerFindById"></a>
# **customerFindById**
> Customer customerFindById(id, filter)

Find a model instance by {{id}} from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Model id
String filter = "filter_example"; // String | Filter defining fields and include
try {
    Customer result = apiInstance.customerFindById(id, filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerFindById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Model id |
 **filter** | **String**| Filter defining fields and include | [optional]

### Return type

[**Customer**](Customer.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerFindOne"></a>
# **customerFindOne**
> Customer customerFindOne(filter)

Find first instance of the model matched by filter from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String filter = "filter_example"; // String | Filter defining fields, where, include, order, offset, and limit
try {
    Customer result = apiInstance.customerFindOne(filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerFindOne");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **String**| Filter defining fields, where, include, order, offset, and limit | [optional]

### Return type

[**Customer**](Customer.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerLogin"></a>
# **customerLogin**
> Object customerLogin(credentials, include)

Login a user with username/email and password.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
Object credentials = null; // Object | 
String include = "include_example"; // String | Related objects to include in the response. See the description of return value for more details.
try {
    Object result = apiInstance.customerLogin(credentials, include);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerLogin");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **credentials** | **Object**|  |
 **include** | **String**| Related objects to include in the response. See the description of return value for more details. | [optional]

### Return type

**Object**

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerLogout"></a>
# **customerLogout**
> customerLogout()

Logout a user with access token.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
try {
    apiInstance.customerLogout();
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerLogout");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerPrototypeCountAccessTokens"></a>
# **customerPrototypeCountAccessTokens**
> InlineResponse200 customerPrototypeCountAccessTokens(id, where)

Counts accessTokens of Customer.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Customer id
String where = "where_example"; // String | Criteria to match model instances
try {
    InlineResponse200 result = apiInstance.customerPrototypeCountAccessTokens(id, where);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerPrototypeCountAccessTokens");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Customer id |
 **where** | **String**| Criteria to match model instances | [optional]

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerPrototypeCountDesigns"></a>
# **customerPrototypeCountDesigns**
> InlineResponse200 customerPrototypeCountDesigns(id, where)

Counts designs of Customer.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Customer id
String where = "where_example"; // String | Criteria to match model instances
try {
    InlineResponse200 result = apiInstance.customerPrototypeCountDesigns(id, where);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerPrototypeCountDesigns");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Customer id |
 **where** | **String**| Criteria to match model instances | [optional]

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerPrototypeCreateAccessTokens"></a>
# **customerPrototypeCreateAccessTokens**
> AccessToken customerPrototypeCreateAccessTokens(id, data)

Creates a new instance in accessTokens of this model.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Customer id
AccessToken data = new AccessToken(); // AccessToken | 
try {
    AccessToken result = apiInstance.customerPrototypeCreateAccessTokens(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerPrototypeCreateAccessTokens");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Customer id |
 **data** | [**AccessToken**](AccessToken.md)|  | [optional]

### Return type

[**AccessToken**](AccessToken.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerPrototypeCreateDesigns"></a>
# **customerPrototypeCreateDesigns**
> Design customerPrototypeCreateDesigns(id, data)

Creates a new instance in designs of this model.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Customer id
Design data = new Design(); // Design | 
try {
    Design result = apiInstance.customerPrototypeCreateDesigns(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerPrototypeCreateDesigns");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Customer id |
 **data** | [**Design**](Design.md)|  | [optional]

### Return type

[**Design**](Design.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerPrototypeDeleteAccessTokens"></a>
# **customerPrototypeDeleteAccessTokens**
> customerPrototypeDeleteAccessTokens(id)

Deletes all accessTokens of this model.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Customer id
try {
    apiInstance.customerPrototypeDeleteAccessTokens(id);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerPrototypeDeleteAccessTokens");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Customer id |

### Return type

null (empty response body)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerPrototypeDeleteDesigns"></a>
# **customerPrototypeDeleteDesigns**
> customerPrototypeDeleteDesigns(id)

Deletes all designs of this model.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Customer id
try {
    apiInstance.customerPrototypeDeleteDesigns(id);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerPrototypeDeleteDesigns");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Customer id |

### Return type

null (empty response body)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerPrototypeDestroyByIdAccessTokens"></a>
# **customerPrototypeDestroyByIdAccessTokens**
> customerPrototypeDestroyByIdAccessTokens(id, fk)

Delete a related item by id for accessTokens.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Customer id
String fk = "fk_example"; // String | Foreign key for accessTokens
try {
    apiInstance.customerPrototypeDestroyByIdAccessTokens(id, fk);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerPrototypeDestroyByIdAccessTokens");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Customer id |
 **fk** | **String**| Foreign key for accessTokens |

### Return type

null (empty response body)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerPrototypeDestroyByIdDesigns"></a>
# **customerPrototypeDestroyByIdDesigns**
> customerPrototypeDestroyByIdDesigns(id, fk)

Delete a related item by id for designs.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Customer id
String fk = "fk_example"; // String | Foreign key for designs
try {
    apiInstance.customerPrototypeDestroyByIdDesigns(id, fk);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerPrototypeDestroyByIdDesigns");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Customer id |
 **fk** | **String**| Foreign key for designs |

### Return type

null (empty response body)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerPrototypeFindByIdAccessTokens"></a>
# **customerPrototypeFindByIdAccessTokens**
> AccessToken customerPrototypeFindByIdAccessTokens(id, fk)

Find a related item by id for accessTokens.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Customer id
String fk = "fk_example"; // String | Foreign key for accessTokens
try {
    AccessToken result = apiInstance.customerPrototypeFindByIdAccessTokens(id, fk);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerPrototypeFindByIdAccessTokens");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Customer id |
 **fk** | **String**| Foreign key for accessTokens |

### Return type

[**AccessToken**](AccessToken.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerPrototypeFindByIdDesigns"></a>
# **customerPrototypeFindByIdDesigns**
> Design customerPrototypeFindByIdDesigns(id, fk)

Find a related item by id for designs.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Customer id
String fk = "fk_example"; // String | Foreign key for designs
try {
    Design result = apiInstance.customerPrototypeFindByIdDesigns(id, fk);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerPrototypeFindByIdDesigns");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Customer id |
 **fk** | **String**| Foreign key for designs |

### Return type

[**Design**](Design.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerPrototypeGetAccessTokens"></a>
# **customerPrototypeGetAccessTokens**
> List&lt;AccessToken&gt; customerPrototypeGetAccessTokens(id, filter)

Queries accessTokens of Customer.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Customer id
String filter = "filter_example"; // String | 
try {
    List<AccessToken> result = apiInstance.customerPrototypeGetAccessTokens(id, filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerPrototypeGetAccessTokens");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Customer id |
 **filter** | **String**|  | [optional]

### Return type

[**List&lt;AccessToken&gt;**](AccessToken.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerPrototypeGetDesigns"></a>
# **customerPrototypeGetDesigns**
> List&lt;Design&gt; customerPrototypeGetDesigns(id, filter)

Queries designs of Customer.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Customer id
String filter = "filter_example"; // String | 
try {
    List<Design> result = apiInstance.customerPrototypeGetDesigns(id, filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerPrototypeGetDesigns");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Customer id |
 **filter** | **String**|  | [optional]

### Return type

[**List&lt;Design&gt;**](Design.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerPrototypeUpdateAttributesPatchCustomersid"></a>
# **customerPrototypeUpdateAttributesPatchCustomersid**
> Customer customerPrototypeUpdateAttributesPatchCustomersid(id, data)

Patch attributes for a model instance and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Customer id
Customer data = new Customer(); // Customer | An object of model property name/value pairs
try {
    Customer result = apiInstance.customerPrototypeUpdateAttributesPatchCustomersid(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerPrototypeUpdateAttributesPatchCustomersid");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Customer id |
 **data** | [**Customer**](Customer.md)| An object of model property name/value pairs | [optional]

### Return type

[**Customer**](Customer.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerPrototypeUpdateAttributesPutCustomersid"></a>
# **customerPrototypeUpdateAttributesPutCustomersid**
> Customer customerPrototypeUpdateAttributesPutCustomersid(id, data)

Patch attributes for a model instance and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Customer id
Customer data = new Customer(); // Customer | An object of model property name/value pairs
try {
    Customer result = apiInstance.customerPrototypeUpdateAttributesPutCustomersid(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerPrototypeUpdateAttributesPutCustomersid");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Customer id |
 **data** | [**Customer**](Customer.md)| An object of model property name/value pairs | [optional]

### Return type

[**Customer**](Customer.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerPrototypeUpdateByIdAccessTokens"></a>
# **customerPrototypeUpdateByIdAccessTokens**
> AccessToken customerPrototypeUpdateByIdAccessTokens(id, fk, data)

Update a related item by id for accessTokens.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Customer id
String fk = "fk_example"; // String | Foreign key for accessTokens
AccessToken data = new AccessToken(); // AccessToken | 
try {
    AccessToken result = apiInstance.customerPrototypeUpdateByIdAccessTokens(id, fk, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerPrototypeUpdateByIdAccessTokens");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Customer id |
 **fk** | **String**| Foreign key for accessTokens |
 **data** | [**AccessToken**](AccessToken.md)|  | [optional]

### Return type

[**AccessToken**](AccessToken.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerPrototypeUpdateByIdDesigns"></a>
# **customerPrototypeUpdateByIdDesigns**
> Design customerPrototypeUpdateByIdDesigns(id, fk, data)

Update a related item by id for designs.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Customer id
String fk = "fk_example"; // String | Foreign key for designs
Design data = new Design(); // Design | 
try {
    Design result = apiInstance.customerPrototypeUpdateByIdDesigns(id, fk, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerPrototypeUpdateByIdDesigns");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Customer id |
 **fk** | **String**| Foreign key for designs |
 **data** | [**Design**](Design.md)|  | [optional]

### Return type

[**Design**](Design.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerReplaceById"></a>
# **customerReplaceById**
> Customer customerReplaceById(id, data)

Replace attributes for a model instance and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String id = "id_example"; // String | Model id
Customer data = new Customer(); // Customer | Model instance data
try {
    Customer result = apiInstance.customerReplaceById(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerReplaceById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Model id |
 **data** | [**Customer**](Customer.md)| Model instance data | [optional]

### Return type

[**Customer**](Customer.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerReplaceOrCreate"></a>
# **customerReplaceOrCreate**
> Customer customerReplaceOrCreate(data)

Replace an existing model instance or insert a new one into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
Customer data = new Customer(); // Customer | Model instance data
try {
    Customer result = apiInstance.customerReplaceOrCreate(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerReplaceOrCreate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Customer**](Customer.md)| Model instance data | [optional]

### Return type

[**Customer**](Customer.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerResetPassword"></a>
# **customerResetPassword**
> customerResetPassword(options)

Reset password for a user with email.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
Object options = null; // Object | 
try {
    apiInstance.customerResetPassword(options);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerResetPassword");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **options** | **Object**|  |

### Return type

null (empty response body)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerUpdateAll"></a>
# **customerUpdateAll**
> InlineResponse2001 customerUpdateAll(where, data)

Update instances of the model matched by {{where}} from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String where = "where_example"; // String | Criteria to match model instances
Customer data = new Customer(); // Customer | An object of model property name/value pairs
try {
    InlineResponse2001 result = apiInstance.customerUpdateAll(where, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerUpdateAll");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **where** | **String**| Criteria to match model instances | [optional]
 **data** | [**Customer**](Customer.md)| An object of model property name/value pairs | [optional]

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerUpsertPatchCustomers"></a>
# **customerUpsertPatchCustomers**
> Customer customerUpsertPatchCustomers(data)

Patch an existing model instance or insert a new one into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
Customer data = new Customer(); // Customer | Model instance data
try {
    Customer result = apiInstance.customerUpsertPatchCustomers(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerUpsertPatchCustomers");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Customer**](Customer.md)| Model instance data | [optional]

### Return type

[**Customer**](Customer.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerUpsertPutCustomers"></a>
# **customerUpsertPutCustomers**
> Customer customerUpsertPutCustomers(data)

Patch an existing model instance or insert a new one into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
Customer data = new Customer(); // Customer | Model instance data
try {
    Customer result = apiInstance.customerUpsertPutCustomers(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerUpsertPutCustomers");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Customer**](Customer.md)| Model instance data | [optional]

### Return type

[**Customer**](Customer.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="customerUpsertWithWhere"></a>
# **customerUpsertWithWhere**
> Customer customerUpsertWithWhere(where, data)

Update an existing model instance or insert a new one into the data source based on the where criteria.

### Example
```java
// Import classes:
//import com.tweak.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String where = "where_example"; // String | Criteria to match model instances
Customer data = new Customer(); // Customer | An object of model property name/value pairs
try {
    Customer result = apiInstance.customerUpsertWithWhere(where, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerUpsertWithWhere");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **where** | **String**| Criteria to match model instances | [optional]
 **data** | [**Customer**](Customer.md)| An object of model property name/value pairs | [optional]

### Return type

[**Customer**](Customer.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

