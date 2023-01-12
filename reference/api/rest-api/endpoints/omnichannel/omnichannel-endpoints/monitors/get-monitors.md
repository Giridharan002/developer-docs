# Get Monitors

Retrieves a list of monitors&#x20;

![](../../../../../../../.gitbook/assets/enterprise.jpg)

| URL                        | Requires Auth | HTTP Method |
| -------------------------- | ------------- | ----------- |
| `api/v1/livechat/monitors` | `YES`         | `GET`       |

## Headers

| Argument       | Example        | Required | Description                                                    |
| -------------- | -------------- | -------- | -------------------------------------------------------------- |
| `X-User-Id`    | `myuser-name`  | Required | Your username hash (returned after you log in through the API) |
| `X-Auth-Token` | `myauth-token` | Required | Your token (returned after you log in through the API)         |

## Example Call

```bash


curl --location --request GET 'http://localhost:3000/api/v1/livechat/monitors' \
--header 'X-Auth-Token: myauth-token' \
--header 'X-User-Id: myuser-name'
```

## Result

```javascript
{
    "monitors": [
        {
            "_id": "gxcJTYapi5mPxuAme",
            "username": "Bruno",
            "emails": [
                {
                    "address": "",
                    "verified": false
                }
            ],
            "status": "offline",
            "name": "Bruno",
            "statusLivechat": "not-available"
        },
        {
            "_id": "QDHWqcubZunM8C4NR",
            "username": "gomes",
            "emails": [
                {
                    "address": "",
                    "verified": true
                }
            ],
            "status": "offline",
            "name": " Gomes",
            "statusLivechat": "not-available"
        },
        
    ],
    "count": 2,
    "offset": 0,
    "total": 2,
    "success": true
}
```
