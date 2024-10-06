# Cloudmersive.APIClient.NETCore.Phishing.Api.PhishingUrlBatchApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**PhishingUrlAdvancedBatchPost**](PhishingUrlBatchApi.md#phishingurladvancedbatchpost) | **POST** /phishing/url/advanced/batch | Accept multiple urls at once to perform lookups to see if the urls are known phishing sites as well as multiple other scans to determine  if the URL is a potential phishing threat.
[**PhishingUrlBatchPost**](PhishingUrlBatchApi.md#phishingurlbatchpost) | **POST** /phishing/url/batch | Accept multiple urls at oncee and perform AI and deterministic methods to detect if a URL is a phishing threat.


<a name="phishingurladvancedbatchpost"></a>
# **PhishingUrlAdvancedBatchPost**
> PhishingUrlAdvancedResponseBatch PhishingUrlAdvancedBatchPost (PhishingUrlAdvancedRequestBatch body = null)

Accept multiple urls at once to perform lookups to see if the urls are known phishing sites as well as multiple other scans to determine  if the URL is a potential phishing threat.

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
    public class PhishingUrlAdvancedBatchPostExample
    {
        public void main()
        {
            // Configure API key authorization: Apikey
            Configuration.Default.AddApiKey("Apikey", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // Configuration.Default.AddApiKeyPrefix("Apikey", "Bearer");

            var apiInstance = new PhishingUrlBatchApi();
            var body = new PhishingUrlAdvancedRequestBatch(); // PhishingUrlAdvancedRequestBatch |  (optional) 

            try
            {
                // Accept multiple urls at once to perform lookups to see if the urls are known phishing sites as well as multiple other scans to determine  if the URL is a potential phishing threat.
                PhishingUrlAdvancedResponseBatch result = apiInstance.PhishingUrlAdvancedBatchPost(body);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling PhishingUrlBatchApi.PhishingUrlAdvancedBatchPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**PhishingUrlAdvancedRequestBatch**](PhishingUrlAdvancedRequestBatch.md)|  | [optional] 

### Return type

[**PhishingUrlAdvancedResponseBatch**](PhishingUrlAdvancedResponseBatch.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/_*+json, application/xml, text/xml, application/_*+xml
 - **Accept**: text/plain, application/json, text/json, application/xml, text/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a name="phishingurlbatchpost"></a>
# **PhishingUrlBatchPost**
> PhishingUrlResponseBatch PhishingUrlBatchPost (List<PhishingUrlRequest> body = null)

Accept multiple urls at oncee and perform AI and deterministic methods to detect if a URL is a phishing threat.

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
    public class PhishingUrlBatchPostExample
    {
        public void main()
        {
            // Configure API key authorization: Apikey
            Configuration.Default.AddApiKey("Apikey", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // Configuration.Default.AddApiKeyPrefix("Apikey", "Bearer");

            var apiInstance = new PhishingUrlBatchApi();
            var body = new List<PhishingUrlRequest>(); // List<PhishingUrlRequest> |  (optional) 

            try
            {
                // Accept multiple urls at oncee and perform AI and deterministic methods to detect if a URL is a phishing threat.
                PhishingUrlResponseBatch result = apiInstance.PhishingUrlBatchPost(body);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling PhishingUrlBatchApi.PhishingUrlBatchPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**List&lt;PhishingUrlRequest&gt;**](PhishingUrlRequest.md)|  | [optional] 

### Return type

[**PhishingUrlResponseBatch**](PhishingUrlResponseBatch.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/_*+json, application/xml, text/xml, application/_*+xml
 - **Accept**: text/plain, application/json, text/json, application/xml, text/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

