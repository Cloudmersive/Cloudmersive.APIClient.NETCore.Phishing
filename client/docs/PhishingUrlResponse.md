# Cloudmersive.APIClient.NETCore.Phishing.Model.PhishingUrlResponse
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CleanResult** | **bool?** | Specifies if the url (or its host or domain) passed all the checks or not. | [optional] 
**Risk** | **double?** | Risk value from 0.0 - 1.0. Higher numbers are a higher risk  &lt;br /&gt;Anything below 0.3 should be considered safe. Anything above 0.7 should be considered a significant risk. &lt;br /&gt;  A score of 1.0 indicates the url, host, or domain failed significant safety checks.&lt;br /&gt;  If a url passes all the tests for the basic api, the risk will be 0.7. If a url passes all the tests for the advanced api, the risk will be 0.2. | [optional] 
**ContainsThreatUrl** | **bool?** | Specifies if the full url with query parameters and fragment is a phishing threat  &lt;br /&gt;The advanced api performs more checks on the full url. | [optional] 
**ContainsThreatHost** | **bool?** | Specifies if the host of the url (i.e. &#x60;&#x60;&#x60;mysite.hostingsite.com&#x60;&#x60;&#x60; for a url of &#x60;&#x60;&#x60;https://mysite.hostingsite.com/index.html&#x60;&#x60;&#x60;) is a phishing threat  &lt;br /&gt;The advanced api performs more checks on the host | [optional] 
**ContainsThreatDomain** | **bool?** | Specifies if the registerable domain of the url (i.e. &#x60;&#x60;&#x60;hostingsite.com&#x60;&#x60;&#x60; for a url of &#x60;&#x60;&#x60;https://mysite.hostingsite.com/index.html&#x60;&#x60;&#x60;) is a phishing threat  &lt;br /&gt;The advanced api performs more checks on the domain | [optional] 
**InputUrl** | **string** | Input URL that was scanned | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

