# UserApi

All URIs are relative to *https://apidevcdn.tweak.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**userConfirm**](UserApi.md#userConfirm) | **GET** /Users/confirm | Confirm a user registration with email verification token.
[**userCount**](UserApi.md#userCount) | **GET** /Users/count | Count instances of the model matched by where from the data source.
[**userCreate**](UserApi.md#userCreate) | **POST** /Users | Create a new instance of the model and persist it into the data source.
[**userCreateChangeStreamGetUsersChangeStream**](UserApi.md#userCreateChangeStreamGetUsersChangeStream) | **GET** /Users/change-stream | Create a change stream.
[**userCreateChangeStreamPostUsersChangeStream**](UserApi.md#userCreateChangeStreamPostUsersChangeStream) | **POST** /Users/change-stream | Create a change stream.
[**userDeleteById**](UserApi.md#userDeleteById) | **DELETE** /Users/{id} | Delete a model instance by {{id}} from the data source.
[**userExistsGetUsersidExists**](UserApi.md#userExistsGetUsersidExists) | **GET** /Users/{id}/exists | Check whether a model instance exists in the data source.
[**userExistsHeadUsersid**](UserApi.md#userExistsHeadUsersid) | **HEAD** /Users/{id} | Check whether a model instance exists in the data source.
[**userFind**](UserApi.md#userFind) | **GET** /Users | Find all instances of the model matched by filter from the data source.
[**userFindById**](UserApi.md#userFindById) | **GET** /Users/{id} | Find a model instance by {{id}} from the data source.
[**userFindOne**](UserApi.md#userFindOne) | **GET** /Users/findOne | Find first instance of the model matched by filter from the data source.
[**userLogin**](UserApi.md#userLogin) | **POST** /Users/login | Login a user with username/email and password.
[**userLogout**](UserApi.md#userLogout) | **POST** /Users/logout | Logout a user with access token.
[**userPrototypeCountAccessTokens**](UserApi.md#userPrototypeCountAccessTokens) | **GET** /Users/{id}/accessTokens/count | Counts accessTokens of User.
[**userPrototypeCreateAccessTokens**](UserApi.md#userPrototypeCreateAccessTokens) | **POST** /Users/{id}/accessTokens | Creates a new instance in accessTokens of this model.
[**userPrototypeDeleteAccessTokens**](UserApi.md#userPrototypeDeleteAccessTokens) | **DELETE** /Users/{id}/accessTokens | Deletes all accessTokens of this model.
[**userPrototypeDestroyByIdAccessTokens**](UserApi.md#userPrototypeDestroyByIdAccessTokens) | **DELETE** /Users/{id}/accessTokens/{fk} | Delete a related item by id for accessTokens.
[**userPrototypeFindByIdAccessTokens**](UserApi.md#userPrototypeFindByIdAccessTokens) | **GET** /Users/{id}/accessTokens/{fk} | Find a related item by id for accessTokens.
[**userPrototypeGetAccessTokens**](UserApi.md#userPrototypeGetAccessTokens) | **GET** /Users/{id}/accessTokens | Queries accessTokens of User.
[**userPrototypeUpdateAttributesPatchUsersid**](UserApi.md#userPrototypeUpdateAttributesPatchUsersid) | **PATCH** /Users/{id} | Patch attributes for a model instance and persist it into the data source.
[**userPrototypeUpdateAttributesPutUsersid**](UserApi.md#userPrototypeUpdateAttributesPutUsersid) | **PUT** /Users/{id} | Patch attributes for a model instance and persist it into the data source.
[**userPrototypeUpdateByIdAccessTokens**](UserApi.md#userPrototypeUpdateByIdAccessTokens) | **PUT** /Users/{id}/accessTokens/{fk} | Update a related item by id for accessTokens.
[**userReplaceById**](UserApi.md#userReplaceById) | **POST** /Users/{id}/replace | Replace attributes for a model instance and persist it into the data source.
[**userReplaceOrCreate**](UserApi.md#userReplaceOrCreate) | **POST** /Users/replaceOrCreate | Replace an existing model instance or insert a new one into the data source.
[**userResetPassword**](UserApi.md#userResetPassword) | **POST** /Users/reset | Reset password for a user with email.
[**userUpdateAll**](UserApi.md#userUpdateAll) | **POST** /Users/update | Update instances of the model matched by {{where}} from the data source.
[**userUpsertPatchUsers**](UserApi.md#userUpsertPatchUsers) | **PATCH** /Users | Patch an existing model instance or insert a new one into the data source.
[**userUpsertPutUsers**](UserApi.md#userUpsertPutUsers) | **PUT** /Users | Patch an existing model instance or insert a new one into the data source.
[**userUpsertWithWhere**](UserApi.md#userUpsertWithWhere) | **POST** /Users/upsertWithWhere | Update an existing model instance or insert a new one into the data source based on the where criteria.


<a name="userConfirm"></a>
# **userConfirm**
> userConfirm(uid, token, redirect)

Confirm a user registration with email verification token.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String uid = "uid_example"; // String | 
String token = "token_example"; // String | 
String redirect = "redirect_example"; // String | 
try {
    apiInstance.userConfirm(uid, token, redirect);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userConfirm");
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

<a name="userCount"></a>
# **userCount**
> InlineResponse200 userCount(where)

Count instances of the model matched by where from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String where = "where_example"; // String | Criteria to match model instances
try {
    InlineResponse200 result = apiInstance.userCount(where);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userCount");
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

<a name="userCreate"></a>
# **userCreate**
> User userCreate(data)

Create a new instance of the model and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
User data = new User(); // User | Model instance data
try {
    User result = apiInstance.userCreate(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userCreate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**User**](User.md)| Model instance data | [optional]

### Return type

[**User**](User.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userCreateChangeStreamGetUsersChangeStream"></a>
# **userCreateChangeStreamGetUsersChangeStream**
> File userCreateChangeStreamGetUsersChangeStream(options)

Create a change stream.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String options = "options_example"; // String | 
try {
    File result = apiInstance.userCreateChangeStreamGetUsersChangeStream(options);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userCreateChangeStreamGetUsersChangeStream");
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

<a name="userCreateChangeStreamPostUsersChangeStream"></a>
# **userCreateChangeStreamPostUsersChangeStream**
> File userCreateChangeStreamPostUsersChangeStream(options)

Create a change stream.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String options = "options_example"; // String | 
try {
    File result = apiInstance.userCreateChangeStreamPostUsersChangeStream(options);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userCreateChangeStreamPostUsersChangeStream");
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

<a name="userDeleteById"></a>
# **userDeleteById**
> Object userDeleteById(id)

Delete a model instance by {{id}} from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String id = "id_example"; // String | Model id
try {
    Object result = apiInstance.userDeleteById(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userDeleteById");
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

<a name="userExistsGetUsersidExists"></a>
# **userExistsGetUsersidExists**
> InlineResponse2002 userExistsGetUsersidExists(id)

Check whether a model instance exists in the data source.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String id = "id_example"; // String | Model id
try {
    InlineResponse2002 result = apiInstance.userExistsGetUsersidExists(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userExistsGetUsersidExists");
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

<a name="userExistsHeadUsersid"></a>
# **userExistsHeadUsersid**
> InlineResponse2002 userExistsHeadUsersid(id)

Check whether a model instance exists in the data source.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String id = "id_example"; // String | Model id
try {
    InlineResponse2002 result = apiInstance.userExistsHeadUsersid(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userExistsHeadUsersid");
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

<a name="userFind"></a>
# **userFind**
> List&lt;User&gt; userFind(filter)

Find all instances of the model matched by filter from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String filter = "filter_example"; // String | Filter defining fields, where, include, order, offset, and limit
try {
    List<User> result = apiInstance.userFind(filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userFind");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **String**| Filter defining fields, where, include, order, offset, and limit | [optional]

### Return type

[**List&lt;User&gt;**](User.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userFindById"></a>
# **userFindById**
> User userFindById(id, filter)

Find a model instance by {{id}} from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String id = "id_example"; // String | Model id
String filter = "filter_example"; // String | Filter defining fields and include
try {
    User result = apiInstance.userFindById(id, filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userFindById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Model id |
 **filter** | **String**| Filter defining fields and include | [optional]

### Return type

[**User**](User.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userFindOne"></a>
# **userFindOne**
> User userFindOne(filter)

Find first instance of the model matched by filter from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String filter = "filter_example"; // String | Filter defining fields, where, include, order, offset, and limit
try {
    User result = apiInstance.userFindOne(filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userFindOne");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter** | **String**| Filter defining fields, where, include, order, offset, and limit | [optional]

### Return type

[**User**](User.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userLogin"></a>
# **userLogin**
> Object userLogin(credentials, include)

Login a user with username/email and password.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
Object credentials = null; // Object | 
String include = "include_example"; // String | Related objects to include in the response. See the description of return value for more details.
try {
    Object result = apiInstance.userLogin(credentials, include);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userLogin");
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

<a name="userLogout"></a>
# **userLogout**
> userLogout()

Logout a user with access token.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
try {
    apiInstance.userLogout();
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userLogout");
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

<a name="userPrototypeCountAccessTokens"></a>
# **userPrototypeCountAccessTokens**
> InlineResponse200 userPrototypeCountAccessTokens(id, where)

Counts accessTokens of User.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String id = "id_example"; // String | User id
String where = "where_example"; // String | Criteria to match model instances
try {
    InlineResponse200 result = apiInstance.userPrototypeCountAccessTokens(id, where);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userPrototypeCountAccessTokens");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| User id |
 **where** | **String**| Criteria to match model instances | [optional]

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userPrototypeCreateAccessTokens"></a>
# **userPrototypeCreateAccessTokens**
> AccessToken userPrototypeCreateAccessTokens(id, data)

Creates a new instance in accessTokens of this model.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String id = "id_example"; // String | User id
AccessToken data = new AccessToken(); // AccessToken | 
try {
    AccessToken result = apiInstance.userPrototypeCreateAccessTokens(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userPrototypeCreateAccessTokens");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| User id |
 **data** | [**AccessToken**](AccessToken.md)|  | [optional]

### Return type

[**AccessToken**](AccessToken.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userPrototypeDeleteAccessTokens"></a>
# **userPrototypeDeleteAccessTokens**
> userPrototypeDeleteAccessTokens(id)

Deletes all accessTokens of this model.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String id = "id_example"; // String | User id
try {
    apiInstance.userPrototypeDeleteAccessTokens(id);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userPrototypeDeleteAccessTokens");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| User id |

### Return type

null (empty response body)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userPrototypeDestroyByIdAccessTokens"></a>
# **userPrototypeDestroyByIdAccessTokens**
> userPrototypeDestroyByIdAccessTokens(id, fk)

Delete a related item by id for accessTokens.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String id = "id_example"; // String | User id
String fk = "fk_example"; // String | Foreign key for accessTokens
try {
    apiInstance.userPrototypeDestroyByIdAccessTokens(id, fk);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userPrototypeDestroyByIdAccessTokens");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| User id |
 **fk** | **String**| Foreign key for accessTokens |

### Return type

null (empty response body)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userPrototypeFindByIdAccessTokens"></a>
# **userPrototypeFindByIdAccessTokens**
> AccessToken userPrototypeFindByIdAccessTokens(id, fk)

Find a related item by id for accessTokens.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String id = "id_example"; // String | User id
String fk = "fk_example"; // String | Foreign key for accessTokens
try {
    AccessToken result = apiInstance.userPrototypeFindByIdAccessTokens(id, fk);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userPrototypeFindByIdAccessTokens");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| User id |
 **fk** | **String**| Foreign key for accessTokens |

### Return type

[**AccessToken**](AccessToken.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userPrototypeGetAccessTokens"></a>
# **userPrototypeGetAccessTokens**
> List&lt;AccessToken&gt; userPrototypeGetAccessTokens(id, filter)

Queries accessTokens of User.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String id = "id_example"; // String | User id
String filter = "filter_example"; // String | 
try {
    List<AccessToken> result = apiInstance.userPrototypeGetAccessTokens(id, filter);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userPrototypeGetAccessTokens");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| User id |
 **filter** | **String**|  | [optional]

### Return type

[**List&lt;AccessToken&gt;**](AccessToken.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userPrototypeUpdateAttributesPatchUsersid"></a>
# **userPrototypeUpdateAttributesPatchUsersid**
> User userPrototypeUpdateAttributesPatchUsersid(id, data)

Patch attributes for a model instance and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String id = "id_example"; // String | User id
User data = new User(); // User | An object of model property name/value pairs
try {
    User result = apiInstance.userPrototypeUpdateAttributesPatchUsersid(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userPrototypeUpdateAttributesPatchUsersid");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| User id |
 **data** | [**User**](User.md)| An object of model property name/value pairs | [optional]

### Return type

[**User**](User.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userPrototypeUpdateAttributesPutUsersid"></a>
# **userPrototypeUpdateAttributesPutUsersid**
> User userPrototypeUpdateAttributesPutUsersid(id, data)

Patch attributes for a model instance and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String id = "id_example"; // String | User id
User data = new User(); // User | An object of model property name/value pairs
try {
    User result = apiInstance.userPrototypeUpdateAttributesPutUsersid(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userPrototypeUpdateAttributesPutUsersid");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| User id |
 **data** | [**User**](User.md)| An object of model property name/value pairs | [optional]

### Return type

[**User**](User.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userPrototypeUpdateByIdAccessTokens"></a>
# **userPrototypeUpdateByIdAccessTokens**
> AccessToken userPrototypeUpdateByIdAccessTokens(id, fk, data)

Update a related item by id for accessTokens.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String id = "id_example"; // String | User id
String fk = "fk_example"; // String | Foreign key for accessTokens
AccessToken data = new AccessToken(); // AccessToken | 
try {
    AccessToken result = apiInstance.userPrototypeUpdateByIdAccessTokens(id, fk, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userPrototypeUpdateByIdAccessTokens");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| User id |
 **fk** | **String**| Foreign key for accessTokens |
 **data** | [**AccessToken**](AccessToken.md)|  | [optional]

### Return type

[**AccessToken**](AccessToken.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userReplaceById"></a>
# **userReplaceById**
> User userReplaceById(id, data)

Replace attributes for a model instance and persist it into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String id = "id_example"; // String | Model id
User data = new User(); // User | Model instance data
try {
    User result = apiInstance.userReplaceById(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userReplaceById");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**| Model id |
 **data** | [**User**](User.md)| Model instance data | [optional]

### Return type

[**User**](User.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userReplaceOrCreate"></a>
# **userReplaceOrCreate**
> User userReplaceOrCreate(data)

Replace an existing model instance or insert a new one into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
User data = new User(); // User | Model instance data
try {
    User result = apiInstance.userReplaceOrCreate(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userReplaceOrCreate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**User**](User.md)| Model instance data | [optional]

### Return type

[**User**](User.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userResetPassword"></a>
# **userResetPassword**
> userResetPassword(options)

Reset password for a user with email.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
Object options = null; // Object | 
try {
    apiInstance.userResetPassword(options);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userResetPassword");
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

<a name="userUpdateAll"></a>
# **userUpdateAll**
> InlineResponse2001 userUpdateAll(where, data)

Update instances of the model matched by {{where}} from the data source.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String where = "where_example"; // String | Criteria to match model instances
User data = new User(); // User | An object of model property name/value pairs
try {
    InlineResponse2001 result = apiInstance.userUpdateAll(where, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userUpdateAll");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **where** | **String**| Criteria to match model instances | [optional]
 **data** | [**User**](User.md)| An object of model property name/value pairs | [optional]

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userUpsertPatchUsers"></a>
# **userUpsertPatchUsers**
> User userUpsertPatchUsers(data)

Patch an existing model instance or insert a new one into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
User data = new User(); // User | Model instance data
try {
    User result = apiInstance.userUpsertPatchUsers(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userUpsertPatchUsers");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**User**](User.md)| Model instance data | [optional]

### Return type

[**User**](User.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userUpsertPutUsers"></a>
# **userUpsertPutUsers**
> User userUpsertPutUsers(data)

Patch an existing model instance or insert a new one into the data source.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
User data = new User(); // User | Model instance data
try {
    User result = apiInstance.userUpsertPutUsers(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userUpsertPutUsers");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**User**](User.md)| Model instance data | [optional]

### Return type

[**User**](User.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

<a name="userUpsertWithWhere"></a>
# **userUpsertWithWhere**
> User userUpsertWithWhere(where, data)

Update an existing model instance or insert a new one into the data source based on the where criteria.

### Example
```java
// Import classes:
//import com.tweak.api.UserApi;

UserApi apiInstance = new UserApi();
String where = "where_example"; // String | Criteria to match model instances
User data = new User(); // User | An object of model property name/value pairs
try {
    User result = apiInstance.userUpsertWithWhere(where, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userUpsertWithWhere");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **where** | **String**| Criteria to match model instances | [optional]
 **data** | [**User**](User.md)| An object of model property name/value pairs | [optional]

### Return type

[**User**](User.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

