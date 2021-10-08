# jwt_api
![image](https://user-images.githubusercontent.com/27144268/136512643-e3ba7dcb-7f6f-4331-b8a4-99cc8a73a636.png)

/Auth/AuthFilters/*
- Action Filters for Authentication & Authorization

/Auth/AuthHelper.cs
* GetToken: To generate token
* IsValidSecretKeys: To validate basic header secret
* ValidateToken: To validate bearer token passed in header.


APIs:
> http://localhost:51893/api/token - to generate token
 
- verb: POST
- header:
  - Authorization : Basic BASE64TOKEN
- Parameters: text/json
  - {"username":"client", "password": "123", "companyId":"123"}




> http://localhost:51893/api/values - to generate token
- verb: GET
- header:
  - Authorization : bearer JWT_TOKEN




