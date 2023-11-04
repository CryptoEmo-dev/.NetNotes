# ASP.NET Core Security

Cookies  for dummies 

A cookie is a small piece of data that is stored in the user's website that is stored on http headers / response, and it have a lot of functions
* Track User's Browsing Activity
* Remembering login details
* Track site visitor count (each cookie has a unique id)

Third party cookies - are set by domains and not the website and is used for cross-site tracking and advertising purposes.


**Authentication ** - Verify you are who you say you are & generate the security context. 
**Security Context ** - All your identity info that is relevant to the facility. 
**Authorization** - Verifying the security context satisfies the access requirements. 

SCENARIO: 
* The login page is where the authentication begins it can be a cookie or token
* After you receive the cookie and login page you will be redirected to the web pages you want with the security context.
* Now authorization will come because depending on your access level you can proceed or not on the desired web pages.





*Now looking at the diagram*
*First, user logins and send http request and the web server logic usually verify the credentials 
* The server side retrieves the database credentials and then generate the SECURITY CONTEXT ( can be token or cookie)
* Then forwarded again on the client side where it will be stored on the headers / response
*  Authentication ( deserialize the cookie to get the security context)
* Once we have the security context then we can tell that if the user's is authorize to access the page
  
![image](https://github.com/CryptoEmo-dev/.NetNotes/assets/123077155/d87f0805-1e8d-4044-87b6-4a9707f6a882)






 
**ASP.NET CORE SECURITY CONTEXT**

*Principal object (USER) - contains one or many identities
Identity - Can be the access levels
Claims - key that pairs your information

![image](https://github.com/CryptoEmo-dev/.NetNotes/assets/123077155/a96f746a-398c-408f-bb9b-eea78d40942d)




 
**
AUTHORIZATION ARCHITECTURE AND FLOW 
**





Cookie Implementation Example 
Middleware as you can see here specifying the CookieName , login path on your program.cs

![image](https://github.com/CryptoEmo-dev/.NetNotes/assets/123077155/fcb4c20a-539e-4fdd-97ce-502fe18ad9cf)



Now create the claims if the condition is true and will be redirected to the protected page 

![image](https://github.com/CryptoEmo-dev/.NetNotes/assets/123077155/cbfa145f-7357-4fbc-8d0c-52fcf947715c)



