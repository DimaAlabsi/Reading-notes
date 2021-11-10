 # Authorization/Authentication
 
 
 
 ## Review, Research, and Discussion
 * What header(s) are used in authentication and authorization
 
The WWW-Authenticate and Proxy-Authenticate response headers define the authentication method that should be used to gain access to a resource. They must specify which authentication scheme is used, so that the client that wishes to authorize knows how to 

* What is safe to put into a JWT


Registered claims like sub , iss , exp or nbf.
Public claims with public names or names registered by IANA which contain values that should be unique like email , address or phone_number . See full list.
Private claims to use in your own context and values can collision

* How are JWTs validated ?

The last segment of a JWT is the signature, which is used to 
verify that the token was signed by the sender and not altered in any way. The Signature is created using the Header and Payload segments, a signing algorithm, and a secret or public key (depending on the chosen signing algorithm)

 
 
 
 
 ## Document the following Vocabulary Terms


|||
|----|------|
|RBAC|Role-based access control (RBAC), also known as role-based security, is a mechanism that restricts system access. It involves setting permissions and privileges to enable access to authorized users. ... Using this table, you can assign permissions to each user|
|User Roles| permission sets that control access to areas and features within the Professional Archive Platform|
|JWT Token|JSON encoded representation of a claim(s) that can be transferred between two parties. The claim is digitally signed by the issuer of the token, and the party receiving this token can later use this digital signature to prove the ownership on the claim|
 

# Preview

Which 3 things had you heard about previously and now have better clarity on?

Authentiacation
   Payload
 Signature  

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
JWT
Linked Lists
Testing

What are you most excited about trying to implement or see how it works? 

continue what we have learned and see the result of those concepts in the front-end with REACT.
 
 #### &copy; Dima Alabsi; 2021
