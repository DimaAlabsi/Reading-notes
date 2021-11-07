


# Bearer Authorization


### Review, Research, and Discussion

1.Write the following steps in the correct order:0
 * Register your application to get a client_id and client_secret
* Ask the client if they want to sign in via a third party
* Redirect to a third party authentication endpoint
* Make a request to a third-party API endpoint
* Receive authorization code
* Make a request to the access token endpoint
* Receive access token

2.What can you do with an authorization code?
**an authorization code is an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space**

3.What can you do with an access token?

access token
***Authorization code flow is used to obtain an access token to authorize API requests. Authorization code flow is the most flexible of the three supported authorization flows and is the recommended method of obtaining an access token for the API.***

What’s a benefit of using OAuth instead of your own basic authentication?

***it enables apps to obtain limited access (scopes) to a user's data without giving away a user's password. It decouples authentication from authorization and supports multiple use cases addressing different device capabilities. It supports server-to-server apps, browser-based apps, mobile/native apps, and consoles/TVs.***

--------------------



## Document the following Vocabulary Terms 


|Term||
|----|-----|
|Client ID|public identifier for apps. Even though it's public, it's best that it isn't guessable by third parties, so many implementations use something like a 32-character hex string. It must also be unique across all clients that the authorization server handles|
|Client Secret|secret known only to your application and the authorization server. It protects your resources by only granting tokens to authorized requestors. Protect your client secrets and never include them in mobile or browser-based apps|
|Authentication Endpoint| security mechanism designed to ensure that only authorized devices can connect to a given network, site or service. The approach is also known as device authentication. ... Authenticating both the user and the device can provide two-factor authentication (2FA|
|Access Token Endpoint||
|API Endpoint||
|Authorization Code||
|Access Token||


## Preview

1.Which 3 things had you heard about previously and now have better clarity on?
2.Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
3.What are you most excited about trying to implement or see how it works?






 #### &copy; Dima Alabsi; 2021
