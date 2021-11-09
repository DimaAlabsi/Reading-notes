# Access Control (ACL)




## Review, Research, and Discussion

1.When is Basic Authorization used vs. Bearer Authorization?
* Bearer Authorization
  * To access the API with a bearer token you will need to make 2 call :
  one to get the bearer token
one to get the data

* Basic Authorization 
    * The basis Auth allow you to access the API directly with your credential : user/password.

 


2.What does the JSON Web Token package do?

* JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.

3.What considerations should we make when creating and storing a SECRET?

* Use encryption to store secrets within .

* Encrypting your secrets using common tools such as git secret and storing them within a git repository can be beneficial when working in teams as it keeps secrets synced

-------------------------------

## Document the following Vocabulary Terms


|||
|----|------|
|encryption|securing digital data using one or more mathematical techniques, along with a password or "key" used to decrypt the information. The encryption process translates information using an algorithm that makes the original information unreadable|
|token| thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user's data. Access tokens must be kept confidential in transit and in storage|
|bearer|predominant type of access token used with OAuth 2.0. A Bearer Token is an opaque string, not intended to have any meaning to clients using it. Some servers will issue tokens that are a short string of hexadecimal characters, while others may use structured tokens such as JSON Web Tokens|
|secret| tools and methods for managing digital authentication credentials (secrets), including passwords, keys, APIs, and tokens for use in applications, services, privileged accounts and other sensitive parts of the IT ecosystem|
|JSON Web Token| a JSON encoded representation of a claim(s) that can be transferred between two parties. The claim is digitally signed by the issuer of the token, and the party receiving this token can later use this digital signature to prove the ownership on the claim|

-----------------------------




## Preview


Which 3 things had you heard about previously and now have better clarity on?

Authentication
access token
express.json

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
middle ware
bearer
Testing

What are you most excited about trying to implement or see how it works?

brear middleware


----------------------


## Preparation Materials 📚

* RBAC is the idea of assigning system access to users based on their role in an organization

* RBAC becomes systematic and repeatable. Further, it is much easier to audit user rights, and to correct any issues identified.

***RBAC vs. ABAC vs. ACL***
|||
|-----|--------|
|Access control lists (ACL)|An ACL is a means of defining access rights by a given user or user group, to a specific object, such as a document.  |
|Attribute-based access control (ABAC) |known as policy-based access control, can use a variety of attributes, including user department, time of day, location of access, type of access required, etc. to determine whether a user’s access request should be granted.|

***RBAC implementation***

|||
|-----|-----|
|1. Inventory your systems|
|2. Analyze your workforce and create roles|
|3. Assign people to roles|
|4. Never make one-off changes|
|5. Audit|

 #### &copy; Dima Alabsi; 2021
