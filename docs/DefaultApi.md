# DefaultApi

All URIs are relative to *https://www.tanzschule-renz.de/tanzplaner*

Method | HTTP request | Description
------------- | ------------- | -------------
[**coursesGet**](DefaultApi.md#coursesGet) | **GET** /courses/ | 
[**entriesGet**](DefaultApi.md#entriesGet) | **GET** /entries/ | 
[**entriesViewIdGet**](DefaultApi.md#entriesViewIdGet) | **GET** /entries/view/{id} | 


<a name="coursesGet"></a>
# **coursesGet**
> CoursesResponse coursesGet(id, withEntries, category, showEntryDetails)



### Example
```java
// Import classes:
import de.tanzschulerenz.tanzplaner.client.ApiClient;
import de.tanzschulerenz.tanzplaner.client.ApiException;
import de.tanzschulerenz.tanzplaner.client.Configuration;
import de.tanzschulerenz.tanzplaner.client.models.*;
import de.tanzschulerenz.tanzplaner.client.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://www.tanzschule-renz.de/tanzplaner");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    Integer id = 56; // Integer | 
    Integer withEntries = 1; // Integer | 
    String category = "category_example"; // String | 
    Integer showEntryDetails = 1; // Integer | 
    try {
      CoursesResponse result = apiInstance.coursesGet(id, withEntries, category, showEntryDetails);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#coursesGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**|  | [optional]
 **withEntries** | **Integer**|  | [optional] [default to 1]
 **category** | **String**|  | [optional]
 **showEntryDetails** | **Integer**|  | [optional] [default to 1]

### Return type

[**CoursesResponse**](CoursesResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |

<a name="entriesGet"></a>
# **entriesGet**
> EntriesResponse entriesGet()



### Example
```java
// Import classes:
import de.tanzschulerenz.tanzplaner.client.ApiClient;
import de.tanzschulerenz.tanzplaner.client.ApiException;
import de.tanzschulerenz.tanzplaner.client.Configuration;
import de.tanzschulerenz.tanzplaner.client.models.*;
import de.tanzschulerenz.tanzplaner.client.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://www.tanzschule-renz.de/tanzplaner");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      EntriesResponse result = apiInstance.entriesGet();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#entriesGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**EntriesResponse**](EntriesResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |

<a name="entriesViewIdGet"></a>
# **entriesViewIdGet**
> EntryResponse entriesViewIdGet(id)



### Example
```java
// Import classes:
import de.tanzschulerenz.tanzplaner.client.ApiClient;
import de.tanzschulerenz.tanzplaner.client.ApiException;
import de.tanzschulerenz.tanzplaner.client.Configuration;
import de.tanzschulerenz.tanzplaner.client.models.*;
import de.tanzschulerenz.tanzplaner.client.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://www.tanzschule-renz.de/tanzplaner");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    Integer id = 56; // Integer | 
    try {
      EntryResponse result = apiInstance.entriesViewIdGet(id);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#entriesViewIdGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**|  |

### Return type

[**EntryResponse**](EntryResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |

