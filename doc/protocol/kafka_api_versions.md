### version 0
```
ApiVersions Request (Version: 0) => 
```
```
ApiVersions Response (Version: 0) => error_code [api_keys] 
  error_code => INT16
  api_keys => api_key min_version max_version 
    api_key => INT16
    min_version => INT16
    max_version => INT16
```
### version 3
```
ApiVersions Request (Version: 3) => client_software_name client_software_version TAG_BUFFER 
  client_software_name => COMPACT_STRING
  client_software_version => COMPACT_STRING
```
```
ApiVersions Response (Version: 3) => error_code [api_keys] throttle_time_ms TAG_BUFFER 
  error_code => INT16
  api_keys => api_key min_version max_version TAG_BUFFER 
    api_key => INT16
    min_version => INT16
    max_version => INT16
  throttle_time_ms => INT32
```
