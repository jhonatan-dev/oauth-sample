# OAuth Sample Application

This repository contains a sample application which demonstrates connecting to Authorize.Net using the OAuth 2.0 authentication standard.

## **How to Use the Sample Application?**

- Clone or download this repository.
- Open solution OAuthDemo.sln in Visual Studio and set OAuthDemo as StartUp project
- Run OAuthDemo.sln from Visual studio to launch the application. Application runs on local IIS server.

![alt text](https://github.com/AuthorizeNet/oauth-sample-app/blob/master/OAuthDemo/Screenshots/Image1.png )

- ClientId and ClientSecret values can be obtained by contacting Authorize.Net support team at [affiliate@authorize.net](mailto:affiliate@authorize.net) and providing a RedirectUri(This is the page that the merchant is redirected back to after granting permissions) for your application.

Sample ClientId and ClientSecret shown in the below screen can be used for the demo purpose and can later be replaced in the code with newly obtained ClientId and ClientSecret.

File - DemoModel.cs

public Demo()

        {

            ClientId = &quot;4dp5b7gRqk&quot;;

            ClientSecret = &quot;fa3a5b16753d09b24bb44243605a4a98&quot;;

![alt text](https://github.com/AuthorizeNet/oauth-sample-app/blob/master/OAuthDemo/Screenshots/Image2.png )

- Click Continue to go to the next step to obtain OAuth code.

![alt text](https://github.com/AuthorizeNet/oauth-sample-app/blob/master/OAuthDemo/Screenshots/Image3.png )

- ClientId and RedirectUri values are used to get OAuth code.
- Check/Uncheck Read and Write boxes to specify the level of access that the application is requesting.
- State value is echoed back in the response to protect against malicious interception.
- Sub value should be oauth.

- Click Redirect to Authorize.net

![alt text](https://github.com/AuthorizeNet/oauth-sample-app/blob/master/OAuthDemo/Screenshots/Image4.png )
