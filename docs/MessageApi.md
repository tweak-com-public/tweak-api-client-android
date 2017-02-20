# MessageApi

All URIs are relative to *https://apidevcdn.tweak.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**messageGreet**](MessageApi.md#messageGreet) | **GET** /Messages/greet | 


<a name="messageGreet"></a>
# **messageGreet**
> InlineResponse2003 messageGreet(msg)



### Example
```java
// Import classes:
//import com.tweak.api.MessageApi;

MessageApi apiInstance = new MessageApi();
String msg = "msg_example"; // String | 
try {
    InlineResponse2003 result = apiInstance.messageGreet(msg);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling MessageApi#messageGreet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **msg** | **String**|  | [optional]

### Return type

[**InlineResponse2003**](InlineResponse2003.md)

### Authorization

[access_token](../README.md#access_token)

### HTTP request headers

 - **Content-Type**: application/json, application/x-www-form-urlencoded, application/xml, text/xml
 - **Accept**: application/json, application/xml, text/xml, application/javascript, text/javascript

