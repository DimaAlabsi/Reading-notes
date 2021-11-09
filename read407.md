


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

4.What’s a benefit of using OAuth instead of your own basic authentication?

***it enables apps to obtain limited access (scopes) to a user's data without giving away a user's password. It decouples authentication from authorization and supports multiple use cases addressing different device capabilities. It supports server-to-server apps, browser-based apps, mobile/native apps, and consoles/TVs.***

--------------------



## Document the following Vocabulary Terms 


|Term||
|----|-----|
|Client ID|public identifier for apps. Even though it's public, it's best that it isn't guessable by third parties, so many implementations use something like a 32-character hex string. It must also be unique across all clients that the authorization server handles|
|Client Secret|secret known only to your application and the authorization server. It protects your resources by only granting tokens to authorized requestors. Protect your client secrets and never include them in mobile or browser-based apps|
|Authentication Endpoint| security mechanism designed to ensure that only authorized devices can connect to a given network, site or service. The approach is also known as device authentication. ... Authenticating both the user and the device can provide two-factor authentication (2FA|
|Access Token Endpoint| are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user’s data.|
|API Endpoint| is one end of a communication channel. When an API interacts with another system, the touchpoints of this communication are considered endpoints|
|Authorization Code|a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server where the user gets a chance to see what the information the client is requesting, and approve or deny the request|
|Access Token|the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user's data. Access tokens must be kept confidential in transit and in storage|


## Preview

1.Which 3 things had you heard about previously and now have better clarity on?
Authentication
Access 
API Endpoint

2.Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
hash
postregs
async & promises
3.What are you most excited about trying to implement or see how it works?
AJAX



# Preparation Materials 👩‍💻

* JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.


* Here are some scenarios where JSON Web Tokens are useful:
   * Information Exchange 
   * Authorization



 * What is the JSON Web Token structure?

     * Header
      * Payload

    * Signature  

![JSON Web Tokens](https://camo.githubusercontent.com/3dfdc1193afbd3ed787bf1d23a3736a6c33a222fecdfc7be462514434a69972b/68747470733a2f2f7777772e6e6f74736f7365637572652e636f6d2f77702d636f6e74656e742f75706c6f6164732f323031362f30352f696d6167653030312e706e67)



"JWTs can be either signed, encrypted or both. If a token is signed, but not encrypted, everyone can read its contents, but when you don't know the private key, you can't change it. Otherwise, the receiver will notice that the signature won't match anymore." ***[READ MORE](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)***

 #### &copy; Dima Alabsi; 2021
