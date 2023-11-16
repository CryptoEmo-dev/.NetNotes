Notes from webapis , https , CRUD EF , Etc.
video:  https://www.linkedin.com/learning/building-web-apis-with-asp-dot-net-core-in-dot-net/http-in-a-nutshell?autoSkip=true&resume=false&u=89213594


**Rest in a Nutshell **
* Design concept
* built on top of http
* Uses uri's to access resources
* Uses http verbs for operations

  Rest Constraints
  * Uniform interface
  * Client-server
  * Stateless
  * Cacheable
  * Layered system
  * Code on demand

    API DESIGN 
FIRST EXAMPLE DESIGN FOR RETRIEVING PRODUCTS
* https://api.hpplussport.com/products
* https://api.hpplussport.com/products/123 --- where 123 an ID
*  https://api.hpplussport.com/products/123/variants --- gives all of the variants
*   https://api.hpplussport.com/products/123/variants/456 --- if you want to take a look of a specific variant again

  REST WITH HTTP VERBS
*GET - READ DATA
*POST - CREATE NEW DATA
* PUT - UPDATE EXISTING DATA
* DELETE - DELETE EXISTING DATA


  Tools for Testing your APIs
postman / fiddler /dev tools


**So the flow usually on APIS are **
ControllerBase -- ApiController --- HttpGet / Get (httpverbs) 


Defining the relationships using the EntityFramework 
On my experience using this or FLUENTAPI
![image](https://github.com/CryptoEmo-dev/.NetNotes/assets/123077155/1a9df2e6-c9ad-409d-b0c6-a7be856d8bdb)



HANDLING ERRORS and some debugging tips 

Testing the API while adding handling errors would show you the exact errors and redirect you to link where you can actually understand the error in depth

![image](https://github.com/CryptoEmo-dev/.NetNotes/assets/123077155/6e15c624-d8fa-4727-926b-7949ad65dbe9)

![image](https://github.com/CryptoEmo-dev/.NetNotes/assets/123077155/88428eac-ab7f-4473-937e-6a10702132e6)




Asynchronous Actions 

![image](https://github.com/CryptoEmo-dev/.NetNotes/assets/123077155/cafc6be5-efe9-4319-9531-f9bc0c3c1f8c)

Easy implementation of async methods on .net ( this can gives your web app performance benefits depending on the apis nature ) 
![image](https://github.com/CryptoEmo-dev/.NetNotes/assets/123077155/a3294390-c06a-4686-9bc7-17cfaaaa629d)




Using EntitState.Modified
![image](https://github.com/CryptoEmo-dev/.NetNotes/assets/123077155/a8f880d9-42a8-4ee0-b5e5-37e6c2d78e39)

![image](https://github.com/CryptoEmo-dev/.NetNotes/assets/123077155/5470dcdb-8d17-4a38-a542-1e43eae8593f)





















  
  
