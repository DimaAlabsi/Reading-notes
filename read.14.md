# Authentication

 * **OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.**


 * ***The simplest example of OAuth is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.***

 * **In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).**

![ authenticate the user](https://images.squarespace-cdn.com/content/v1/53959e41e4b032d797ff3dc3/1551415047882-3XTPO3V1ASQ1JTLE75R0/user-authentication-process-explained.png)


 * OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans

 ![OAuth vs. OpenID](https://pbs.twimg.com/media/Bxb1iKACcAAnl_2.jpg)




|| Authentication    | Authorization |
|-----------| ----------- | ----------- |
|What does it do?|   Verifies credentials |   Grants or denies permissions  |
| How does it work?|Through passwords, biometrics, one-time pins, or apps||
|Is it visible to the user?|yes|NO|
|It is changeable by the user?|Partially|NO|
|How does data move?|Through ID tokens|Through access tokens |

"
Authorization code flow is used to obtain an access token to authorize API requests. Authorization code flow is the most flexible of the three supported authorization flows and is the recommended method of obtaining an access token for the API. This authorization flow is best suited to applications that have access to secure, private storage such as web applications deployed on a server. Other authorization flows are available to obtain an access token that may be suitable for your application.

Access tokens, obtained using authorization code flow, provide permissions for your application to manipulate documents and other resources on behalf of a Mendeley user and make requests for all API resources. Access tokens while having a limited lifetime, can be renewed with a refresh token. A refresh token is valid indefinitely and provides ability for your application to schedule tasks on behalf of a user without their interaction.
    "  [MEDELEY](https://dev.mendeley.com/reference/topics/authorization_auth_code.html)

* **The Authorization Code Flow + PKCE is an OpenId Connect flow specifically designed to authenticate native or mobile application users.**

"
* Implicit Flow with Form Post flow uses OIDC to implement web sign-in that is very similar to the way SAML and WS-Federation operates. The web app requests and obtains tokens through the front channel, without the need for secrets or extra backend calls. With this method, you don’t need to obtain, maintain, use, and protect a secret in your application.

* Client Credentials Flow
With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user. For this scenario, typical authentication schemes like username + password or social logins don't make sense. Instead, M2M apps use the Client Credentials Flow (defined in OAuth 2.0 RFC 6749, section 4.4), in which they pass along their Client ID and Client Secret to authenticate themselves and get a token.

* With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device. This avoids a poor user experience for devices that do not have an easy way to enter text. To do this, device apps use the Device Authorization Flow (ratified in OAuth 2.0), in which they pass along their Client ID to initiate the authorization process and get a token.

* Though we do not recommend it, highly-trusted applications can use the Resource Owner Password Flow (defined in OAuth 2.0 RFC 6749, section 4.3), which requests that users provide credentials (username and password), typically using an interactive form. Because credentials are sent to the backend and can be stored for future use before being exchanged for an Access Token, it is imperative that the application is absolutely trusted with this information.



" [READ MORE](https://auth0.com/docs/authorization/flows/implicit-flow-with-form-post)




 #### &copy; Dima Alabsi; 2021 
