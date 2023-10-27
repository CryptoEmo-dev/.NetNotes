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



![image](https://github.com/CryptoEmo-dev/.NetNotes/assets/123077155/f766176d-df60-40b9-82fd-d51cd063f7c9)
