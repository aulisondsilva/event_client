# EventClient::Event

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**event_id** | **Integer** | Required in case of update | [optional] 
**project_name** | **String** |  | [required] 
**process_name** | **String** |  | [required] 
**status** | **String** | started, success, aborted, error | [required] 
**error_type** | **String** |  | [optional] 
**error_description** | **String** |  | [optional] 
**server_id** | **String** |  | [optional] 
**lan_ip** | **String** |  | [optional] 
**wan_ip** | **String** |  | [optional] 
**progress** | **Integer** |  | [optional] 
**execution_time** | **Integer** |  | [optional] 
**start_time** | **Integer** | required at add event | [optional] 
**end_time** | **Integer** |  | [optional] 


