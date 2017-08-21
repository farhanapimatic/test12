# 



## Base URL

The Base URL for this API is `http://adsabs.harvard.edu/`



## Authentication
This API uses `OAuth v2.0` with `Client Credentials` grant type.

**Access Token URL:** `/fhsdjfhsd  fsduifh iodfhsdifh oifhisdf h` 



### Scopes

The API makes use of the following OAuth scopes: 

| Name | Value | Description |
| ---- | ----- | ----------- |
| fdg | dfg | TODO: add a description |
| dfg | dfg | TODO: add a description |





# <a name="api_reference"></a>API Reference

* [BibcodeQueryBinding](#bibcode_query_binding)
* [OAuth Authorization](#o_auth_authorization)

## <a name="bibcode_query_binding"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "BibcodeQueryBinding") BibcodeQueryBinding


### <a name="get_bibcode"></a>![Endpoint: ](https://apidocs.io/img/method.png "getBibcode") getBibcode


**`GET`** `/cgi-bin/nph-bib_query`

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description




#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| -------------------------------- |
| bibcode | [string](#api_types) |  ``` Required ```  | TODO: Add a parameter description | `"bibcode"` | 
| db_key | [string](#api_types) |  ``` Required ```  | TODO: Add a parameter description | `"db_key"` | 
| data_type | [string](#api_types) |  ``` Required ```  | TODO: Add a parameter description | `"data_type"` | 

#### Responses
**200** 


Body ([returnBibcode](#return_bibcode)) 
```
{
  "body": "body"
}
```


[Back to API Reference](#api_reference)

## <a name="o_auth_authorization"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "OAuth Authorization") OAuth Authorization


### <a name="request_token"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token") request token


**`POST`** `/fhsdjfhsd  fsduifh iodfhsdifh oifhisdf h`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"client_credentials"` | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = client_credentials 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 62,
  "scope": "scope",
  "expiry": 62
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token1"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token1") request token1


**`POST`** `/fhsdjfhsd  fsduifh iodfhsdifh oifhisdf h`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"client_credentials"` | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = client_credentials 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 62,
  "scope": "scope",
  "expiry": 62
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token2"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token2") request token2


**`POST`** `/fhsdjfhsd  fsduifh iodfhsdifh oifhisdf h`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"client_credentials"` | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = client_credentials 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 62,
  "scope": "scope",
  "expiry": 62
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token11"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token11") request token11


**`POST`** `/fhsdjfhsd  fsduifh iodfhsdifh oifhisdf h`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"client_credentials"` | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = client_credentials 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 245,
  "scope": "scope",
  "expiry": 245
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token21"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token21") request token21


**`POST`** `/fhsdjfhsd  fsduifh iodfhsdifh oifhisdf h`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"client_credentials"` | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = client_credentials 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 245,
  "scope": "scope",
  "expiry": 245
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token11"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token11") request token11


**`POST`** `/fhsdjfhsd  fsduifh iodfhsdifh oifhisdf h`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"client_credentials"` | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = client_credentials 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 245,
  "scope": "scope",
  "expiry": 245
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token1"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token1") request token1


**`POST`** `/fhsdjfhsd  fsduifh iodfhsdifh oifhisdf h`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"client_credentials"` | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = client_credentials 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 245,
  "scope": "scope",
  "expiry": 245
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token2"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token2") request token2


**`POST`** `/fhsdjfhsd  fsduifh iodfhsdifh oifhisdf h`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"client_credentials"` | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = client_credentials 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 245,
  "scope": "scope",
  "expiry": 245
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token3"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token3") request token3


**`POST`** `/fhsdjfhsd  fsduifh iodfhsdifh oifhisdf h`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"client_credentials"` | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = client_credentials 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 245,
  "scope": "scope",
  "expiry": 245
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


### <a name="request_token"></a>![Endpoint: ](https://apidocs.io/img/method.png "request token") request token


**`POST`** `/fhsdjfhsd  fsduifh iodfhsdifh oifhisdf h`

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.




#### Request Headers
>Content-Type=application/x-www-form-urlencoded;
>Authorization="Authorization";

#### Request Body
Url Encoded

> Additional optional form parameters are allowed

| Parameter | Type | Tags | Description | Default Value |
|-----------|------| ---- |-------------| ------------- | 
| grant_type | [string](#api_types) |  ```Constant ```  ``` Required ```  | Grant Type | `"client_credentials"` | 
| scope | [string](#api_types) |  ``` Optional ```  | Requested scopes as a space-delimited list. |  | 

##### Example
```
 grant_type = client_credentials 
 scope = "scope" 
```

#### Responses
**200** 


Body ([OAuthToken](#o_auth_token)) 
```
{
  "access_token": "access_token",
  "token_type": "token_type",
  "expires_in": 245,
  "scope": "scope",
  "expiry": 245
}
```


**400** 

> OAuth 2 provider returned an error.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```
**401** 

> OAuth 2 provider says client authentication failed.

Body ([OAuthProvider](#o_auth_provider)) 
```
{
  "error": "invalid_request",
  "error_description": "error_description",
  "error_uri": "error_uri"
}
```


[Back to API Reference](#api_reference)

## <a name="api_types"></a>![Models: ](https://apidocs.io/img/class.png "API Types") API Types

This section provides details on the available types. The primitive types available are:

| Type | Example |
| ---- | -------- |
| **string** | `hello world` |
| **boolean** |	`true` |
| **number** | `1` |
| **precision** | `1.5` |
| **datetime** | `2016-03-13T12:52:32.123Z` |
| **date** | `2016-03-13` |
|**void** | |
| **dynamic** | |
| **binary** | |
| **long** | `12345678910` |
| **file** | |
| **uuid** | `0f8fad5b-d9cb-469f-a165-70867728950e` |


In addition to the above types, the following complex types are also available:
### <a name="return_bibcode"></a>![Model: ](https://apidocs.io/img/method.png "returnBibcode") returnBibcode



> TODO: Add a method description




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| body | [string](#api_types) |  ``` Required ```  | TODO: Add a property description | 




### <a name="o_auth_scope"></a>![Model: ](https://apidocs.io/img/method.png "OAuth Scope") OAuth Scope



> OAuth 2 scopes supported by the API




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `dfg` | TODO: Add description | 
| `dfg` | TODO: Add description | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_scope"></a>![Model: ](https://apidocs.io/img/method.png "OAuth Scope") OAuth Scope



> OAuth 2 scopes supported by the API




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `dfg` | TODO: Add description | 
| `dfg` | TODO: Add description | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_scope"></a>![Model: ](https://apidocs.io/img/method.png "OAuth Scope") OAuth Scope



> OAuth 2 scopes supported by the API




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `dfg` | TODO: Add description | 
| `dfg` | TODO: Add description | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_scope"></a>![Model: ](https://apidocs.io/img/method.png "OAuth Scope") OAuth Scope



> OAuth 2 scopes supported by the API




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `dfg` | TODO: Add description | 
| `dfg` | TODO: Add description | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_scope"></a>![Model: ](https://apidocs.io/img/method.png "OAuth Scope") OAuth Scope



> OAuth 2 scopes supported by the API




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `dfg` | TODO: Add description | 
| `dfg` | TODO: Add description | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_scope"></a>![Model: ](https://apidocs.io/img/method.png "OAuth Scope") OAuth Scope



> OAuth 2 scopes supported by the API




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `dfg` | TODO: Add description | 
| `dfg` | TODO: Add description | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_scope"></a>![Model: ](https://apidocs.io/img/method.png "OAuth Scope") OAuth Scope



> OAuth 2 scopes supported by the API




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `dfg` | TODO: Add description | 
| `dfg` | TODO: Add description | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_scope"></a>![Model: ](https://apidocs.io/img/method.png "OAuth Scope") OAuth Scope



> OAuth 2 scopes supported by the API




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `dfg` | TODO: Add description | 
| `dfg` | TODO: Add description | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_scope"></a>![Model: ](https://apidocs.io/img/method.png "OAuth Scope") OAuth Scope



> OAuth 2 scopes supported by the API




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `dfg` | TODO: Add description | 
| `dfg` | TODO: Add description | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. | 




### <a name="o_auth_scope"></a>![Model: ](https://apidocs.io/img/method.png "OAuth Scope") OAuth Scope



> OAuth 2 scopes supported by the API




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `dfg` | TODO: Add description | 
| `dfg` | TODO: Add description | 




### <a name="o_auth_token"></a>![Model: ](https://apidocs.io/img/method.png "OAuthToken") OAuthToken



> OAuth 2 Authorization endpoint response




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| access_token | [string](#api_types) |  ``` Required ```  | Access token | 
| token_type | [string](#api_types) |  ``` Required ```  | Type of access token | 
| expires_in | [long](#api_types) |  ``` Optional ```  | Time in seconds before the access token expires | 
| scope | [string](#api_types) |  ``` Optional ```  | List of scopes granted<br>This is a space-delimited list of strings. | 
| expiry | [long](#api_types) |  ``` Optional ```  | Time of token expiry as unix timestamp (UTC) | 




### <a name="o_auth_provider"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProvider") OAuthProvider



> OAuth 2 Authorization endpoint exception




| Name | Type | Tags | Description |
|-----------|------| ---- |-------------| 
| error | [OAuthProviderError](#o_auth_provider_error) |  ``` Required ```  | Error code | 
| error_description | [string](#api_types) |  ``` Optional ```  | Human-readable text providing additional information on error.<br>Used to assist the client developer in understanding the error that occurred. | 
| error_uri | [string](#api_types) |  ``` Optional ```  | A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error | 




### <a name="o_auth_provider_error"></a>![Model: ](https://apidocs.io/img/method.png "OAuthProviderError") OAuthProviderError



> OAuth 2 Authorization error codes




This type must take a value from the following [string](#api_types) enumeration of values:

| Value | Description |
| ----- | --------------- |
| `invalid_request` | The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed. | 
| `invalid_client` | Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method). | 
| `invalid_grant` | The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client. | 
| `unauthorized_client` | The authenticated client is not authorized to use this authorization grant type. | 
| `unsupported_grant_type` | The authorization grant type is not supported by the authorization server. | 
| `invalid_scope` | The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner. |

