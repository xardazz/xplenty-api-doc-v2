## Delete Account

### Description
Delete an existing [account](https://github.com/xplenty/xplenty-api-doc-v2/blob/master/resources/account.md). The operation can be executed only by the account owner.

### Notes
* Please note that this action is **irreversible**.

### Input Parameters
The **account ID** must be supplied at the end of the request URL.

### Request (Curl Call) Syntax
```shell
$ curl -X DELETE -u api_key: "https://api.xplenty.com/accounts/:account_id" \
  -H "Accept: application/vnd.xplenty+json, version=2"
```

### Response Example
```HTTP
HTTP/1.1 200 OK
```

```json
{
  "id":1,
  "account_id":"xplenty-admin",
  "name":"Xplenty Admin",
  "uname": "u_1",
  "region":"amazon-web-services::us-east-1",
  "location":null,
  "billing_email":"admin@xplenty.com",
  "gravatar_email":"admin@xplenty.com",
  "avatar_url":"http://gravatar.com/avatar/d41d8cd98f00b204e9800998ecf8427e.png?d=retro&s=140",
  "created_at":"2015-02-04T12:51:04Z",
  "updated_at":"2015-02-04T12:51:04Z",
  "schedules_count":0,
  "connections_count":0,
  "role":"admin",
  "owner_id":1,
  "members_count":1,
  "packages_count":0,
  "jobs_count":0,
  "running_jobs_count":0,
  "hooks_count":0,
  "url":"https://api.xplenty.com/accounts/xplenty-admin",
  "public_key":"ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAAAgQCoBCkf9FTqBktQlAVLPAC7eMftuaAcxKtPwPPK/mwEAF0Xx7s0AgbsYws8MTsZyMic3aQxDMDn0gZYPOO6ws9+Fk51dBXCWVTgJMB7a01RdmHOV6nX4VNKnc5NRfB8bM8hvWm1UoeIUW6EAsFFiXlwnkLHcodjTjt/LxCXGZftjw== xplenty2@example.com"
}
```
