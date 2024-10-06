# Cloudmersive.APIClient.NETCore.Phishing - the C# library for the phishingapi

Easily and directly scan and block phishing security threats.

This C# SDK is for the [Cloudmersive Phishing Detection API](https://www.cloudmersive.com/phishing-api):

- API version: v1
- SDK version: 1.0.0
- Build package: io.swagger.codegen.languages.CSharpClientCodegen

<a name="frameworks-supported"></a>
## Frameworks supported
- .NET Core >=1.0
- .NET Framework >=4.6
- Mono/Xamarin >=vNext
- UWP >=10.0

<a name="dependencies"></a>
## Dependencies
- FubarCoder.RestSharp.Portable.Core >=4.0.7
- FubarCoder.RestSharp.Portable.HttpClient >=4.0.7
- Newtonsoft.Json >=10.0.3

<a name="installation"></a>
## Installation
Generate the DLL using your preferred tool

Then include the DLL (under the `bin` folder) in the C# project, and use the namespaces:
```csharp
using Cloudmersive.APIClient.NETCore.Phishing.Api;
using Cloudmersive.APIClient.NETCore.Phishing.Client;
using Cloudmersive.APIClient.NETCore.Phishing.Model;
```
<a name="getting-started"></a>
## Getting Started

```csharp
using System;
using System.Diagnostics;
using Cloudmersive.APIClient.NETCore.Phishing.Api;
using Cloudmersive.APIClient.NETCore.Phishing.Client;
using Cloudmersive.APIClient.NETCore.Phishing.Model;

namespace Example
{
    public class Example
    {
        public void main()
        {

            // Configure API key authorization: Apikey
            Configuration.Default.ApiKey.Add("Apikey", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // Configuration.Default.ApiKeyPrefix.Add("Apikey", "Bearer");

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

<a name="documentation-for-api-endpoints"></a>
## Documentation for API Endpoints

All URIs are relative to *https://localhost*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*PhishingUrlApi* | [**PhishingUrlAdvancedPost**](docs/PhishingUrlApi.md#phishingurladvancedpost) | **POST** /phishing/url/advanced | Use advanced AI detection to determine if a URL is a known phishing threat
*PhishingUrlApi* | [**PhishingUrlPost**](docs/PhishingUrlApi.md#phishingurlpost) | **POST** /phishing/url | Use AI and deterministic detection to determine if a URL is a phishing threat
*PhishingUrlBatchApi* | [**PhishingUrlAdvancedBatchPost**](docs/PhishingUrlBatchApi.md#phishingurladvancedbatchpost) | **POST** /phishing/url/advanced/batch | Accept multiple urls at once to perform lookups to see if the urls are known phishing sites as well as multiple other scans to determine  if the URL is a potential phishing threat.
*PhishingUrlBatchApi* | [**PhishingUrlBatchPost**](docs/PhishingUrlBatchApi.md#phishingurlbatchpost) | **POST** /phishing/url/batch | Accept multiple urls at oncee and perform AI and deterministic methods to detect if a URL is a phishing threat.


<a name="documentation-for-models"></a>
## Documentation for Models

 - [Model.PhishingUrlAdvancedRequest](docs/PhishingUrlAdvancedRequest.md)
 - [Model.PhishingUrlAdvancedRequestBatch](docs/PhishingUrlAdvancedRequestBatch.md)
 - [Model.PhishingUrlAdvancedResponse](docs/PhishingUrlAdvancedResponse.md)
 - [Model.PhishingUrlAdvancedResponseBatch](docs/PhishingUrlAdvancedResponseBatch.md)
 - [Model.PhishingUrlRequest](docs/PhishingUrlRequest.md)
 - [Model.PhishingUrlResponse](docs/PhishingUrlResponse.md)
 - [Model.PhishingUrlResponseBatch](docs/PhishingUrlResponseBatch.md)


<a name="documentation-for-authorization"></a>
## Documentation for Authorization

<a name="Apikey"></a>
### Apikey

- **Type**: API key
- **API key parameter name**: Apikey
- **Location**: HTTP header

