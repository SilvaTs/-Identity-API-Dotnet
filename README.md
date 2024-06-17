

###  Demo Identity API Endpoints .NET 8

### Create User Request

```js
POST /identity/register
```

```json
{
  "email": "user@teste.com",
  "password": "senha2924"
}
```

### Create User Response

```js
201 Created
```

```json
{
  "type": "string",
  "title": "string",
  "status": 0,
  "detail": "string",
  "instance": "string",
  "errors": {
    "additionalProp1": [
      "string"
    ],
    "additionalProp2": [
      "string"
    ],
    "additionalProp3": [
      "string"
    ]
  },
  "additionalProp1": "string",
  "additionalProp2": "string",
  "additionalProp3": "string"
}
```

### Login User Request

```js
POST /identity/login
```

```json
{
  "email": "user@teste.com",
  "password": "senha2924"
}
```

### Login User Response

```js
201 Created
```

```json
{
  "tokenType": "Bearer",
  "accessToken": "CfDJ8I-UGSIbCpBLu64BXKvor_puQVodv7jC7P_K-W4o0LCGwB7K7MY7d95Mr4UoQt2TbTDhsJnAXzU7pV1cuLMX3Tl5ZBWQDYvHbL8AxclUeZhjXKhX4yX1chkBCPBemGx6EASdPWi5zzjR-0SZUa-3JdkMi54nEta8dyKMqMfybv6LMkAGnPTOIPLkVfrwk4aH4AqgzxJAAluYBRr4aOASUBpdTwvP5xOsdAt2888zXbTanmLnO5B4cXyMQdUpxbH-INkBnwuIXEWI7KRfz7IolTWF2XESZG9Den0enRwLkQGbbwYKG1QwbLmomQWr0YYxHzBNbfuIeh1fo5QuwZihwRZnacGpO0-9jGuQyXhiGLFMaP-1jIpcdrqCzXhIAGnZn1BMw0zGZ5gRjdzX8W1H_er9SQPFzQ-8ER3KcpfUyXbInEh-Uuq2Zv7Y4BXtMb2KnDPcX-QHWmR2-OTn0iAp29QoxZGFCHqpsyFtrHlvhRLPd0YTbIGJ1ksL4EI2PSfWXo7_5H-vMg5Q9Bd_ppzq8FdF-hT3pMuck-sSxUaZl4r2b7KPUKlyI6_g3L_yivj6m8f0aWcZlDAwS8tjkNsMXDizVZld9ngT6YaSNdpsoa2dGQypYOzHp_GQMYgLbz0QweKOE5RMCrW0FbZfF993Os2OEx9Y0SNqH7klxFFpc0BFDB5jwo3cy7JbAJLaeaussQ",
  "expiresIn": 3600,
  "refreshToken": "CfDJ8I-UGSIbCpBLu64BXKvor_qkKTQAfe6tuebDoAs_QSd6bg9Q6xON-GWnVXLHfoZzX-lbwqA4-G1p0N0MVQfaGtisvQdZox6ouygwb1BH-IRyOgmpMWjLK_gdWVIKah2rOINSQWwfdJkDbPQLVGo2ggBzw17CBczVG9rQ4hY7e1CSv-PyI3RQqS9iO7bawiQVpkm6FO54jxbz7XH_NgQItWlY9FC_-xT-lecUz-Bv88N0eln5L9y3hggcfP2lxLRZzb7IwoPIb6DNWkwmXfI_lHL-bq7eGw_dbHIZZYWmY4vZw3sBK36_fNYFUfwO6WviFCqKxgEuaSGAY95ozhumnw7QopFCMg1yaNt32fzmIOi3YygDr1iOAqcLql2NehcyZQDmRc3qEq0zA6orjUntstgXIouCwovP6WKSFQELfsUcpniUsrF92o0xYh2ZMjcI1HmMBDX-yB-vqye3QeTRZG7j0vmJ4eNTxIHBqJdK4Re8gsGAqKdmSCiNDKluE-zlvZU4dqMHDk83CxRT_9RNxVmpnqeqP38eHXoOlz_nHxRS4onID4omsUyZTX5PUVARFVd2W_TNKP_XJzg4uHY7WsWbmgrjAXV5oU-cos8nkhf1ZKhMwBmg2uksQ8fic1SWf4QsheXTrMpob_qn5-yqqvGg8tOGhBVu06xesvm0oeoR7TBOAcOwCMHhFWr5u2jr7A"
}
```

### Refresh Token Request

```js
POST /identity/refresh
```

```json
{
  "refreshToken": "myRefreshToken"
}
```

### Refresh Token Response

```js
201 Created
```

```json
{
  "tokenType": "Bearer",
  "accessToken": "CfDJ8I-UGSIbCpBLu64BXKvor_puQVodv7jC7P_K-W4o0LCGwB7K7MY7d95Mr4UoQt2TbTDhsJnAXzU7pV1cuLMX3Tl5ZBWQDYvHbL8AxclUeZhjXKhX4yX1chkBCPBemGx6EASdPWi5zzjR-0SZUa-3JdkMi54nEta8dyKMqMfybv6LMkAGnPTOIPLkVfrwk4aH4AqgzxJAAluYBRr4aOASUBpdTwvP5xOsdAt2888zXbTanmLnO5B4cXyMQdUpxbH-INkBnwuIXEWI7KRfz7IolTWF2XESZG9Den0enRwLkQGbbwYKG1QwbLmomQWr0YYxHzBNbfuIeh1fo5QuwZihwRZnacGpO0-9jGuQyXhiGLFMaP-1jIpcdrqCzXhIAGnZn1BMw0zGZ5gRjdzX8W1H_er9SQPFzQ-8ER3KcpfUyXbInEh-Uuq2Zv7Y4BXtMb2KnDPcX-QHWmR2-OTn0iAp29QoxZGFCHqpsyFtrHlvhRLPd0YTbIGJ1ksL4EI2PSfWXo7_5H-vMg5Q9Bd_ppzq8FdF-hT3pMuck-sSxUaZl4r2b7KPUKlyI6_g3L_yivj6m8f0aWcZlDAwS8tjkNsMXDizVZld9ngT6YaSNdpsoa2dGQypYOzHp_GQMYgLbz0QweKOE5RMCrW0FbZfF993Os2OEx9Y0SNqH7klxFFpc0BFDB5jwo3cy7JbAJLaeaussQ",
  "expiresIn": 3600,
  "refreshToken": "CfDJ8I-UGSIbCpBLu64BXKvor_qkKTQAfe6tuebDoAs_QSd6bg9Q6xON-GWnVXLHfoZzX-lbwqA4-G1p0N0MVQfaGtisvQdZox6ouygwb1BH-IRyOgmpMWjLK_gdWVIKah2rOINSQWwfdJkDbPQLVGo2ggBzw17CBczVG9rQ4hY7e1CSv-PyI3RQqS9iO7bawiQVpkm6FO54jxbz7XH_NgQItWlY9FC_-xT-lecUz-Bv88N0eln5L9y3hggcfP2lxLRZzb7IwoPIb6DNWkwmXfI_lHL-bq7eGw_dbHIZZYWmY4vZw3sBK36_fNYFUfwO6WviFCqKxgEuaSGAY95ozhumnw7QopFCMg1yaNt32fzmIOi3YygDr1iOAqcLql2NehcyZQDmRc3qEq0zA6orjUntstgXIouCwovP6WKSFQELfsUcpniUsrF92o0xYh2ZMjcI1HmMBDX-yB-vqye3QeTRZG7j0vmJ4eNTxIHBqJdK4Re8gsGAqKdmSCiNDKluE-zlvZU4dqMHDk83CxRT_9RNxVmpnqeqP38eHXoOlz_nHxRS4onID4omsUyZTX5PUVARFVd2W_TNKP_XJzg4uHY7WsWbmgrjAXV5oU-cos8nkhf1ZKhMwBmg2uksQ8fic1SWf4QsheXTrMpob_qn5-yqqvGg8tOGhBVu06xesvm0oeoR7TBOAcOwCMHhFWr5u2jr7A"
}
```









