# Cloudmersive.APIClient.NETCore.Phishing.Api.PhishingUrlApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**PhishingUrlAdvancedPost**](PhishingUrlApi.md#phishingurladvancedpost) | **POST** /phishing/url/advanced | Use advanced AI detection to determine if a URL is a known phishing threat
[**PhishingUrlPost**](PhishingUrlApi.md#phishingurlpost) | **POST** /phishing/url | Use AI and deterministic detection to determine if a URL is a phishing threat


<a name="phishingurladvancedpost"></a>
# **PhishingUrlAdvancedPost**
> PhishingUrlAdvancedResponse PhishingUrlAdvancedPost (PhishingUrlAdvancedRequest body = null)

Use advanced AI detection to determine if a URL is a known phishing threat

Uses advanced AI and deterministic methods to detect if a URL is a phishing threat.

### Example
```csharp
using System;
using System.Diagnostics;
using Cloudmersive.APIClient.NETCore.Phishing.Api;
using Cloudmersive.APIClient.NETCore.Phishing.Client;
using Cloudmersive.APIClient.NETCore.Phishing.Model;

namespace Example
{
    public class PhishingUrlAdvancedPostExample
    {
        public void main()
        {
            // Configure API key authorization: Apikey
            Configuration.Default.AddApiKey("Apikey", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // Configuration.Default.AddApiKeyPrefix("Apikey", "Bearer");

            var apiInstance = new PhishingUrlApi();
            var body = new PhishingUrlAdvancedRequest(); // PhishingUrlAdvancedRequest |  (optional) 

            try
            {
                // Use advanced AI detection to determine if a URL is a known phishing threat
                PhishingUrlAdvancedResponse result = apiInstance.PhishingUrlAdvancedPost(body);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling PhishingUrlApi.PhishingUrlAdvancedPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**PhishingUrlAdvancedRequest**](PhishingUrlAdvancedRequest.md)|  | [optional] 

### Return type

[**PhishingUrlAdvancedResponse**](PhishingUrlAdvancedResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/_*+json, application/xml, text/xml, application/_*+xml
 - **Accept**: text/plain, application/json, text/json, application/xml, text/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="phishingurlpost"></a>
# **PhishingUrlPost**
> PhishingUrlResponse PhishingUrlPost (PhishingUrlRequest body = null)

Use AI and deterministic detection to determine if a URL is a phishing threat

Uses AI and deterministic methods to detect if a URL is a phishing threat.

### Example
```csharp
using System;
using System.Diagnostics;
using Cloudmersive.APIClient.NETCore.Phishing.Api;
using Cloudmersive.APIClient.NETCore.Phishing.Client;
using Cloudmersive.APIClient.NETCore.Phishing.Model;

namespace Example
{
    public class PhishingUrlPostExample
    {
        public void main()
        {
            // Configure API key authorization: Apikey
            Configuration.Default.AddApiKey("Apikey", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // Configuration.Default.AddApiKeyPrefix("Apikey", "Bearer");

            var apiInstance = new PhishingUrlApi();
            var body = new PhishingUrlRequest(); // PhishingUrlRequest |  (optional) 

            try
            {
                // Use AI and deterministic detection to determine if a URL is a phishing threat
                PhishingUrlResponse result = apiInstance.PhishingUrlPost(body);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling PhishingUrlApi.PhishingUrlPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**PhishingUrlRequest**](PhishingUrlRequest.md)|  | [optional] 

### Return type

[**PhishingUrlResponse**](PhishingUrlResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/_*+json, application/xml, text/xml, application/_*+xml
 - **Accept**: text/plain, application/json, text/json, application/xml, text/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

