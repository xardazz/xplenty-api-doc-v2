## List available Regions

### Description
This call returns information for the list of regions supported by Xplenty. You can also select regions for particular Brand.
You can use this information to verify the regions in which you can create a cluster.

### Input Parameters

|Name|Required?|Default|Description|
|----|---------|-------|-----------|
brand_id|N| |The Brand's numeric identifier for which you want to list regions.

### Request (Curl Call) Syntax
```shell
$curl -X GET -u api_key: "https://api.xplenty.com/regions?brand_id=1" \
  -H "Accept: application/vnd.xplenty+json; version=2"
```

### Response Example
```HTTP
HTTP/1.1 200 OK
```

```json
[
  {
    "name": "AWS - Us East (N. Virginia)",
    "group_name": "Amazon Web Services",
    "id": "amazon-web-services::us-east-1"
  },
  {
    "name": "Rackspace - Dallas (DFW)",
    "group_name": "Rackspace Cloud Servers",
    "id": "rackspace::dfw"
  },
  {
    "name": "Google Cloud",
    "group_name": "Google Cloud - US (Central)",
    "id": "us-central1"
  }
]
```
