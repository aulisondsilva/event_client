# EventClient::RegisterEventApi

All URIs are relative to *http://eventservice.marketcheck.com:8986/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_event**](RegisterEventApi.md#add_event) | **POST** /register_event | Register a new event
[**update_event**](RegisterEventApi.md#update_event) | **POST** /update_event | Register a new event


# **add_event**
> Object add_event(body)

Register a new event



### Example
```ruby
# load the gem
require 'event_client'

api_instance = EventClient::RegisterEventApi.new

body = EventClient::Event.new # Event | Event object that needs to be added to the Index


begin
  #Register a new event
  result = api_instance.add_event(body)
  p result
rescue EventClient::ApiError => e
  puts "Exception when calling RegisterEventApi->add_event: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Event**](Event.md)| Event object that needs to be added to the Index | 

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **update_event**
> Object update_event(body)

Register a new event



### Example
```ruby
# load the gem
require 'event_client'

api_instance = EventClient::RegisterEventApi.new

body = EventClient::Event.new # Event | Event object that needs to be added to the Index


begin
  #Register a new event
  result = api_instance.update_event(body)
  p result
rescue EventClient::ApiError => e
  puts "Exception when calling RegisterEventApi->update_event: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Event**](Event.md)| Event object that needs to be added to the Index | 

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



