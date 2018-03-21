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

body = body =   {
                   project_name: "Export",
                   process_name: "Autobot Export One Day",
                   status: "started",
                   server_id: "server name",
                   lan_ip: "xx.xx.xx.xx",
                   wan_ip: "xxx.xx.xxx.xxx",
                   start_time: "Timestamp in utc""
                }
 # Event | Event object that needs to be added to the Index


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

body =   {
            event_id: "87654567890987654321234567890",
            project_name: "Export",
            process_name: "Autobot Export One Day",
            status: "started",
            server_id: "server name",
            lan_ip: "xx.xx.xx.xx",
            wan_ip: "xxx.xx.xxx.xxx",
            start_time: "Timestamp in utc",
            progress: 40
         } 
 # Event | Event object that needs to be added to the Index


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



