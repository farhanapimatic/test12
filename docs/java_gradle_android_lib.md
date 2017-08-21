# Getting started

## How to Build

The generated code uses a few Gradle dependencies e.g., Jackson, Volley,
and Apache HttpClient. The reference to these dependencies is already
added in the build.gradle file will be installed automatically. Therefore,
you will need internet access for a successful build.

* In order to open the client library in Android Studio click on ``` Open an Existing Android Project ```.

![Importing SDK into Android Studio - Step 1](https://apidocs.io/illustration/android?step=import1&workspaceFolder=BibcodeQuery&workspaceName=BibcodeQuery&projectName=BibcodeQueryLib&rootNamespace=edu.harvard.adsabs)

* Browse to locate the folder containing the source code. Select the location of the BibcodeQuery gradle project and click ``` Ok ```.

![Importing SDK into Android Studio - Step 2](https://apidocs.io/illustration/android?step=import2&workspaceFolder=BibcodeQuery&workspaceName=BibcodeQuery&projectName=BibcodeQueryLib&rootNamespace=edu.harvard.adsabs)

* Upon successful import, the project can be built by clicking on ``` Build > Make Project ``` or  pressing ``` Ctrl + F9 ```.

![Importing SDK into Android Studio - Step 3](https://apidocs.io/illustration/android?step=import3&workspaceFolder=BibcodeQuery&workspaceName=BibcodeQuery&projectName=BibcodeQueryLib&rootNamespace=edu.harvard.adsabs)

## How to Use

The following section explains how to use the BibcodeQuery library in a new project.

### 1. Starting a new project 

For starting a new project, click on ``` Create New Android Studio Project ```.

![Add a new project in Android Studio - Step 1](https://apidocs.io/illustration/android?step=createNewProject0&workspaceFolder=BibcodeQuery&workspaceName=BibcodeQuery&projectName=BibcodeQueryLib&rootNamespace=edu.harvard.adsabs)

Here, configure the new project by adding the name, domain and location of the sample application followed by clicking ``` Next ```.

![Create a new Android Studio Project - Step 2](https://apidocs.io/illustration/android?step=createNewProject1&workspaceFolder=BibcodeQuery&workspaceName=BibcodeQuery&projectName=BibcodeQueryLib&rootNamespace=edu.harvard.adsabs)

Following this, select the ``` Phone and Tablet ```` option as shown in the illustration below and click ``` Next ```. 

![Create a new Android Studio Project - Step 3](https://apidocs.io/illustration/android?step=createNewProject2&workspaceFolder=BibcodeQuery&workspaceName=BibcodeQuery&projectName=BibcodeQueryLib&rootNamespace=edu.harvard.adsabs)

In the following step, choose ``` Empty Activity ``` as the activity type and click ``` Next ```.

![Create a new Android Studio Project - Step 4](https://apidocs.io/illustration/android?step=createNewProject3&workspaceFolder=BibcodeQuery&workspaceName=BibcodeQuery&projectName=BibcodeQueryLib&rootNamespace=edu.harvard.adsabs)

In this step, provide an ``` Activity Name ``` and ``` Layout Name ``` and click ``` Finish ```.  This would take you to the newly created project.

![Create a new Android Studio Project - Step 4](https://apidocs.io/illustration/android?step=createNewProject4&workspaceFolder=BibcodeQuery&workspaceName=BibcodeQuery&projectName=BibcodeQueryLib&rootNamespace=edu.harvard.adsabs)

### 2. Add reference of the library project

In order to add a dependency to this sample application, click on the android button shown in the project explorer on the left side as shown in the picture. Click on ``` Project ``` in the drop down that emerges.  

![Adding dependency to the client library - Step 1](https://apidocs.io/illustration/android?step=testProject0&workspaceFolder=BibcodeQuery&workspaceName=BibcodeQuery&projectName=BibcodeQueryLib&rootNamespace=edu.harvard.adsabs)

Right click the sample application in the project explorer and click on ``` New > Module ```  as shown in the picture.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/android?step=testProject1&workspaceFolder=BibcodeQuery&workspaceName=BibcodeQuery&projectName=BibcodeQueryLib&rootNamespace=edu.harvard.adsabs)

Choose ``` Import Gradle Project ``` and click ``` Next ```.

![Adding dependency to the client library - Step 3](https://apidocs.io/illustration/android?step=testProject2&workspaceFolder=BibcodeQuery&workspaceName=BibcodeQuery&projectName=BibcodeQueryLib&rootNamespace=edu.harvard.adsabs)

Click on ``` Finish ``` which would take you back to the sample application with the refernced SDK. 

![Adding dependency to the client library - Step 4](https://apidocs.io/illustration/android?step=testProject3&workspaceFolder=BibcodeQuery&workspaceName=BibcodeQuery&projectName=BibcodeQueryLib&rootNamespace=edu.harvard.adsabs)

In the following step naigate to the ``` SampleApplication >  app > build.gradle ``` file and add the following line ```compile project(path: ':BibcodeQuery')``` to the dependencies section as shown in the illustration below.

![Adding dependency to the client library - Step 5](https://apidocs.io/illustration/android?step=testProject4&workspaceFolder=BibcodeQuery&workspaceName=BibcodeQuery&projectName=BibcodeQueryLib&rootNamespace=edu.harvard.adsabs)

Finally, press ``` Sync Now ``` in the warning visible as shown in the picture below.

![Adding dependency to the client library - Step 6](https://apidocs.io/illustration/android?step=testProject5&workspaceFolder=BibcodeQuery&workspaceName=BibcodeQuery&projectName=BibcodeQueryLib&rootNamespace=edu.harvard.adsabs)

### 3. Write sample code

Once the ``` SampleApplication ``` is created, a file named ``` SampleApplication > app > src > main > java > MainActivity ``` will be visible in the *Project Explorer* with an ``` onCreate ``` method. This is the entry point for the execution of the created project.
Here, you can add code to initialize the client library and instantiate a *Controller* class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

## How to Test

The generated code and the server can be tested using automatically generated test cases. 
JUnit is used as the testing framework and test runner.

In Android Studio, for running the tests do the following:

1. Right click on *SampleApplication > BibcodeQueryLib > androidTest > java)* from the project explorer.
2. Select "Run All Tests" or use "Ctrl + Shift + F10" to run the Tests.

## Initialization

### Authentication
In order to setup authentication and initialization of the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| oAuthClientId | OAuth 2 Client ID |
| oAuthClientSecret | OAuth 2 Client Secret |



API client can be initialized as following. The `appContext` being passed is the Android application [`Context`](https://developer.android.com/reference/android/content/Context.html).

```java
// Configuration parameters and credentials
String oAuthClientId = "oAuthClientId"; // OAuth 2 Client ID
String oAuthClientSecret = "oAuthClientSecret"; // OAuth 2 Client Secret

edu.harvard.adsabs.Configuration.initialize(appContext);
BibcodeQueryClient client = new BibcodeQueryClient(oAuthClientId, oAuthClientSecret);
```

You must authorize now authorize the client.

### Authorizing your client

This SDK uses *OAuth 2.0 authorization* to authorize the client.

The `authorize()` method will exchange the OAuth client credentials for an *access token*.
The access token is an object containing information for authorizing client requests.

 You must pass the *[scopes](#scopes)* for which you need permission to access.
```java
client.auth().authorize(scopes, null, new APICallBack<OAuthToken>() {
                    
    @Override
    public void onSuccess(HttpContext context, OAuthToken response) {
        // TODO Do something after the client is authorized
    }
                    
    @Override
    public void onFailure(HttpContext context, Throwable error) {
        // TODO Handle failure
    }
});
```

The client can now make authorized endpoint calls.


### Scopes

Scopes enable your application to only request access to the resources it needs while enabling users to control the amount of access they grant to your application. Available scopes are defined in the `edu.harvard.adsabs.Models.OAuthScopeEnum` enumeration.

| Scope Name | Description |
| --- | --- |
| `FDG` |  |
| `DFG` |  |

### Storing an access token for reuse

It is recommended that you store the access token for reuse.

```java
// store token in some way
storeAccessToken(edu.harvard.adsabs.Configuration.oAuthToken);
```

### Creating a client from a stored token

To authorize a client from a stored access token, just set the access token in `Configuration` along with the other configuration parameters before creating the client:

```java
// load token later...
edu.harvard.adsabs.Configuration.oAuthToken = loadAccessToken();

// Set other configuration, then instantiate client
BibcodeQueryClient client = new BibcodeQueryClient();
```


# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [BibcodeQueryBindingController](#bibcode_query_binding_controller)
* [OAuthAuthorizationController](#o_auth_authorization_controller)

## <a name="bibcode_query_binding_controller"></a>![Class: ](https://apidocs.io/img/class.png "edu.harvard.adsabs.controllers.BibcodeQueryBindingController") BibcodeQueryBindingController

### Get singleton instance

The singleton instance of the ``` BibcodeQueryBindingController ``` class can be accessed from the API Client.

```java
BibcodeQueryBindingController bibcodeQueryBinding = client.getBibcodeQueryBinding();
```

### <a name="get_bibcode_async"></a>![Method: ](https://apidocs.io/img/method.png "edu.harvard.adsabs.controllers.BibcodeQueryBindingController.getBibcodeAsync") getBibcodeAsync

> *Tags:*  ``` Skips Authentication ``` 

> TODO: Add a method description


```java
void getBibcodeAsync(
        final String bibcode,
        final String dbKey,
        final String dataType,
        final APICallBack<ReturnBibcode> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| bibcode |  ``` Required ```  | TODO: Add a parameter description |
| dbKey |  ``` Required ```  | TODO: Add a parameter description |
| dataType |  ``` Required ```  | TODO: Add a parameter description |


#### Example Usage

```java
String bibcode = "bibcode";
String dbKey = "db_key";
String dataType = "data_type";
// Invoking the API call with sample inputs
bibcodeQueryBinding.getBibcodeAsync(bibcode, dbKey, dataType, new APICallBack<ReturnBibcode>() {
    public void onSuccess(HttpContext context, ReturnBibcode response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)

## <a name="o_auth_authorization_controller"></a>![Class: ](https://apidocs.io/img/class.png "edu.harvard.adsabs.controllers.OAuthAuthorizationController") OAuthAuthorizationController

### Get singleton instance

The singleton instance of the ``` OAuthAuthorizationController ``` class can be accessed from the API Client.

```java
OAuthAuthorizationController oAuthAuthorization = client.getOAuthAuthorization();
```

### <a name="create_request_token_async"></a>![Method: ](https://apidocs.io/img/method.png "edu.harvard.adsabs.controllers.OAuthAuthorizationController.createRequestTokenAsync") createRequestTokenAsync

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.


```java
void createRequestTokenAsync(
        final String authorization,
        final String scope,
        Map<String, Object> fieldParameters,
        final APICallBack<OAuthToken> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| authorization |  ``` Required ```  | Authorization header in Basic auth format |
| scope |  ``` Optional ```  | Requested scopes as a space-delimited list. |
| fieldParameters | ``` Optional ``` | Additional optional form parameters are supported by this method |


#### Example Usage

```java
String authorization = "Authorization";
String scope = "scope";
// key-value map for optional form parameters
Map<String, Object> formParams = new LinkedHashMap<String, Object>();
// Invoking the API call with sample inputs
oAuthAuthorization.createRequestTokenAsync(authorization, scope, formParams, new APICallBack<OAuthToken>() {
    public void onSuccess(HttpContext context, OAuthToken response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 400 | OAuth 2 provider returned an error. |
| 401 | OAuth 2 provider says client authentication failed. |



### <a name="create_request_token1_async"></a>![Method: ](https://apidocs.io/img/method.png "edu.harvard.adsabs.controllers.OAuthAuthorizationController.createRequestToken1Async") createRequestToken1Async

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.


```java
void createRequestToken1Async(
        final String authorization,
        final String scope,
        Map<String, Object> fieldParameters,
        final APICallBack<OAuthToken> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| authorization |  ``` Required ```  | Authorization header in Basic auth format |
| scope |  ``` Optional ```  | Requested scopes as a space-delimited list. |
| fieldParameters | ``` Optional ``` | Additional optional form parameters are supported by this method |


#### Example Usage

```java
String authorization = "Authorization";
String scope = "scope";
// key-value map for optional form parameters
Map<String, Object> formParams = new LinkedHashMap<String, Object>();
// Invoking the API call with sample inputs
oAuthAuthorization.createRequestToken1Async(authorization, scope, formParams, new APICallBack<OAuthToken>() {
    public void onSuccess(HttpContext context, OAuthToken response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 400 | OAuth 2 provider returned an error. |
| 401 | OAuth 2 provider says client authentication failed. |



### <a name="create_request_token2_async"></a>![Method: ](https://apidocs.io/img/method.png "edu.harvard.adsabs.controllers.OAuthAuthorizationController.createRequestToken2Async") createRequestToken2Async

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.


```java
void createRequestToken2Async(
        final String authorization,
        final String scope,
        Map<String, Object> fieldParameters,
        final APICallBack<OAuthToken> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| authorization |  ``` Required ```  | Authorization header in Basic auth format |
| scope |  ``` Optional ```  | Requested scopes as a space-delimited list. |
| fieldParameters | ``` Optional ``` | Additional optional form parameters are supported by this method |


#### Example Usage

```java
String authorization = "Authorization";
String scope = "scope";
// key-value map for optional form parameters
Map<String, Object> formParams = new LinkedHashMap<String, Object>();
// Invoking the API call with sample inputs
oAuthAuthorization.createRequestToken2Async(authorization, scope, formParams, new APICallBack<OAuthToken>() {
    public void onSuccess(HttpContext context, OAuthToken response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 400 | OAuth 2 provider returned an error. |
| 401 | OAuth 2 provider says client authentication failed. |



### <a name="create_request_token11_async"></a>![Method: ](https://apidocs.io/img/method.png "edu.harvard.adsabs.controllers.OAuthAuthorizationController.createRequestToken11Async") createRequestToken11Async

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.


```java
void createRequestToken11Async(
        final String authorization,
        final String scope,
        Map<String, Object> fieldParameters,
        final APICallBack<OAuthToken> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| authorization |  ``` Required ```  | Authorization header in Basic auth format |
| scope |  ``` Optional ```  | Requested scopes as a space-delimited list. |
| fieldParameters | ``` Optional ``` | Additional optional form parameters are supported by this method |


#### Example Usage

```java
String authorization = "Authorization";
String scope = "scope";
// key-value map for optional form parameters
Map<String, Object> formParams = new LinkedHashMap<String, Object>();
// Invoking the API call with sample inputs
oAuthAuthorization.createRequestToken11Async(authorization, scope, formParams, new APICallBack<OAuthToken>() {
    public void onSuccess(HttpContext context, OAuthToken response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 400 | OAuth 2 provider returned an error. |
| 401 | OAuth 2 provider says client authentication failed. |



### <a name="create_request_token21_async"></a>![Method: ](https://apidocs.io/img/method.png "edu.harvard.adsabs.controllers.OAuthAuthorizationController.createRequestToken21Async") createRequestToken21Async

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.


```java
void createRequestToken21Async(
        final String authorization,
        final String scope,
        Map<String, Object> fieldParameters,
        final APICallBack<OAuthToken> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| authorization |  ``` Required ```  | Authorization header in Basic auth format |
| scope |  ``` Optional ```  | Requested scopes as a space-delimited list. |
| fieldParameters | ``` Optional ``` | Additional optional form parameters are supported by this method |


#### Example Usage

```java
String authorization = "Authorization";
String scope = "scope";
// key-value map for optional form parameters
Map<String, Object> formParams = new LinkedHashMap<String, Object>();
// Invoking the API call with sample inputs
oAuthAuthorization.createRequestToken21Async(authorization, scope, formParams, new APICallBack<OAuthToken>() {
    public void onSuccess(HttpContext context, OAuthToken response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 400 | OAuth 2 provider returned an error. |
| 401 | OAuth 2 provider says client authentication failed. |



### <a name="create_request_token1_async"></a>![Method: ](https://apidocs.io/img/method.png "edu.harvard.adsabs.controllers.OAuthAuthorizationController.createRequestToken1Async") createRequestToken1Async

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.


```java
void createRequestToken1Async(
        final String authorization,
        final String scope,
        Map<String, Object> fieldParameters,
        final APICallBack<OAuthToken> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| authorization |  ``` Required ```  | Authorization header in Basic auth format |
| scope |  ``` Optional ```  | Requested scopes as a space-delimited list. |
| fieldParameters | ``` Optional ``` | Additional optional form parameters are supported by this method |


#### Example Usage

```java
String authorization = "Authorization";
String scope = "scope";
// key-value map for optional form parameters
Map<String, Object> formParams = new LinkedHashMap<String, Object>();
// Invoking the API call with sample inputs
oAuthAuthorization.createRequestToken1Async(authorization, scope, formParams, new APICallBack<OAuthToken>() {
    public void onSuccess(HttpContext context, OAuthToken response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 400 | OAuth 2 provider returned an error. |
| 401 | OAuth 2 provider says client authentication failed. |



### <a name="create_request_token_async"></a>![Method: ](https://apidocs.io/img/method.png "edu.harvard.adsabs.controllers.OAuthAuthorizationController.createRequestTokenAsync") createRequestTokenAsync

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.


```java
void createRequestTokenAsync(
        final String authorization,
        final String scope,
        Map<String, Object> fieldParameters,
        final APICallBack<OAuthToken> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| authorization |  ``` Required ```  | Authorization header in Basic auth format |
| scope |  ``` Optional ```  | Requested scopes as a space-delimited list. |
| fieldParameters | ``` Optional ``` | Additional optional form parameters are supported by this method |


#### Example Usage

```java
String authorization = "Authorization";
String scope = "scope";
// key-value map for optional form parameters
Map<String, Object> formParams = new LinkedHashMap<String, Object>();
// Invoking the API call with sample inputs
oAuthAuthorization.createRequestTokenAsync(authorization, scope, formParams, new APICallBack<OAuthToken>() {
    public void onSuccess(HttpContext context, OAuthToken response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 400 | OAuth 2 provider returned an error. |
| 401 | OAuth 2 provider says client authentication failed. |



### <a name="create_request_token_async"></a>![Method: ](https://apidocs.io/img/method.png "edu.harvard.adsabs.controllers.OAuthAuthorizationController.createRequestTokenAsync") createRequestTokenAsync

> *Tags:*  ``` Skips Authentication ``` 

> Create a new OAuth 2 token.


```java
void createRequestTokenAsync(
        final String authorization,
        final String scope,
        Map<String, Object> fieldParameters,
        final APICallBack<OAuthToken> callBack)
```

#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| authorization |  ``` Required ```  | Authorization header in Basic auth format |
| scope |  ``` Optional ```  | Requested scopes as a space-delimited list. |
| fieldParameters | ``` Optional ``` | Additional optional form parameters are supported by this method |


#### Example Usage

```java
String authorization = "Authorization";
String scope = "scope";
// key-value map for optional form parameters
Map<String, Object> formParams = new LinkedHashMap<String, Object>();
// Invoking the API call with sample inputs
oAuthAuthorization.createRequestTokenAsync(authorization, scope, formParams, new APICallBack<OAuthToken>() {
    public void onSuccess(HttpContext context, OAuthToken response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```

#### Errors

| Error Code | Error Description |
|------------|-------------------|
| 400 | OAuth 2 provider returned an error. |
| 401 | OAuth 2 provider says client authentication failed. |



[Back to List of Controllers](#list_of_controllers)



