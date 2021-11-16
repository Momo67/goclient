# AHelloWorldServer.DefaultApi

All URIs are relative to *//localhost:8080/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**helloworldHandler**](DefaultApi.md#helloworldHandler) | **GET** /hello | Handler for returning a HelloWorld message

<a name="helloworldHandler"></a>
# **helloworldHandler**
> &#x27;String&#x27; helloworldHandler(opts)

Handler for returning a HelloWorld message

Simple http handler to give some personalised greetings with a valid html

### Example
```javascript
import {AHelloWorldServer} from 'a_hello_world_server';

let apiInstance = new AHelloWorldServer.DefaultApi();
let opts = { 
  'username': "username_example" // String | Name of user to be welcome
};
apiInstance.helloworldHandler(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **username** | **String**| Name of user to be welcome | [optional] 

### Return type

**&#x27;String&#x27;**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

