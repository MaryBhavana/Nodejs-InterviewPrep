1. What is NPM?
  
   NPM (Node Package Manager) is the default package manager for Node.js and is written entirely in Javascript.
  
   NPM manages all the packages and modules for Node.js and consists of command line client npm. 
  
   It gets installed into the system with installation of Node.js. 
  
   The required packages and modules in Node project are installed using NPM.
  
   A package contains all the files needed for a module and modules are the JavaScript libraries that can be included in Node project according to the 
   requirement of the project.
   
   NPM can install all the dependencies of a project through the package.json file. It can also update and uninstall packages.
  
   To install NPM, it is required to install Node.js as NPM gets installed with Node.js automatically.
           Install Node.js.
           
  _____________________________________________________________________________________________________________________________________________________________
  
 2. What are the modules in Node.js?
 
    Modules can be a single file or a collection of multiples files/folders. 
    The reason programmers are heavily reliant on modules is because of their re-usability as well as the ability to break down a complex piece of code
    into manageable chunks.
    
    Modules are of three types:
   
    - Core Modules        : Node.js has many built-in modules that are part of the platform and comes with Node.js installation. 
                              These modules can be loaded into the program by using the require function.The require() function will
                              return a JavaScript type depending on what the particular module returns.
                              
    - local Modules       :  local modules are created locally in your Node.js application.
        
    - Third-party Modules :  Third-party modules are modules that are available online using the Node Package Manager(NPM). 
                               These modules can be installed in the project folder or globally. Some of the popular third-party modules are mongoose, express, 
                               angular, and react.
                               
 ________________________________________________________________________________________________________________________________________________________________
    
  3. What is the purpose of the module.exports?
  
     - Module.exports are the instruction that tells Node. js which bits of code (functions, objects, strings, etc.) 
       to “export” from a given file so other files are allowed to access the exported code.
       
     - The module.exports is actually a property of the module object in node.js. module. 
     
     - Exports is the object that is returned to the require() call. By module.exports, we can export functions, objects, and their 
       references from one file and can use them in other files by importing them by require() method.
       
      - Easy to maintain and manage the code base in different modules.
      
_____________________________________________________________________________________________________________________________________________________________________

  4. Difference between default export and named export?
  
     ES6 provides two ways to export a module from a file: named export and default export.

         Named Export: (export)

           With named exports, one can have multiple named exports per file. 
           Then import the specific exports they want surrounded in braces. 
      
           The name of imported module has to be the same as the name of the exported module.
           
           Named exports are useful to export several values. During the import, one will be able to use the
           same name to refer to the corresponding value.
           
         Default Export: (export default)

           One can have only one default export per file. When we import we have to specify a name and import.
           
           The naming of import is completely independent in default export and we can use any name we like.
           
           Default export, there is only a single default export per module. A default export can be a function, a 
           class, an object or anything else. This value is to be considered as the “main” exported value since it will 
           be the simplest to import.
         
________________________________________________________________________________________________________________________________________________________________

   5. How do you import any module in Node.js
   
      Importing functions or modules enhances the reusability of code.
      
      Importing a Module: We need to import the module to use the functions defined in the imported module in another file.
      
      The result returned by require() is stored in a variable which is used to invoke the functions using the dot notation.
      
_______________________________________________________________________________________________________________________________________________________________

   6. What are the different types of HTTP requests?
   
      HTTP (Hypertext Transfer Protocol) specifies a collection of request methods to specify what 
      action is to be performed on a particular resource.
      
      The most commonly used HTTP request methods are GET, POST, PUT, PATCH, and DELETE. 
      
      These are equivalent to the CRUD operations (create, read, update, and delete).
      
          GET: GET request is used to read/retrieve data from a web server. GET returns an HTTP status code of
               200 (OK) if the data is successfully retrieved from the server.

          POST: POST request is used to send data (file, form data, etc.) to the server. 
                On successful creation, it returns an HTTP status code of 201.

          PUT: A PUT request is used to modify the data on the server. It replaces the entire content at a particular location with 
              data that is passed in the body payload. If there are no resources that match the request, it will generate one.

          PATCH: PATCH is similar to PUT request, but the only difference is, it modifies a part of the data.
               It will only replace the content that you want to update.

          DELETE: A DELETE request is used to delete the data on the server at a specified location.
          
______________________________________________________________________________________________________________________________________________________________

   7. Explain the concept of middleware in Node.js.
   
      Express.js is a routing and Middleware framework for handling the different routing of 
      the webpage and it works between the request and response cycle.

      Middleware gets executed after the server receives the request and before the controller actions send the response.

      Middleware has the access to the request object, responses object, and next, it can process the request 
        before the server send a response. An Express-based application is a series of middleware function calls.

      Middleware Chaining: Middleware can be chained from one to another, Hence creating a chain of functions 
        that are executed in order. The last function sends the response back to the browser. So, before sending the 
        response back to the browser the different middleware process the request.

      The next() function in the express is responsible for calling the next middleware function if there is one.
         app.get(path, (req, res, next) => {}, (req, res) => {})
         
______________________________________________________________________________________________________________________________________________________________
   
    8. Explain CORS
      
       CORS (Cross-Origin Resource Sharing) is a mechanism by which data or any other resource of a site 
       could be shared intentionally to a third party website when there is a need. Generally, access to resources that are 
       residing in a third party site is restricted by the browser clients for security purposes.
       
_____________________________________________________________________________________________________________________________________________________________

   9. What is Express. how it helps you to create a backend application
   
      Express.js: Express is a small framework that sits on top of Node.js’s web server functionality to simplify its 
      APIs and add helpful new features. It makes it easier to organize your application’s functionality with middle ware 
      and routing. 
      It adds helpful utilities to Node.js’s HTTP objects. It facilitates the rendering of dynamic HTTP objects.

      - More features than Node.js

      - It is used to build web-apps using approaches and principles of Node.js.

      - Routing is provided.

      - It requires less coding time.

      - Uses middleware for the arrangement of functions systematically server-side.

      - import by const express = require ("express")
      
_____________________________________________________________________________________________________________________________________________________________

   10. Explain min 5 status codes gets used in Backend development
   
       - 400 BAD_REQUEST Bad Request 
       
       - 401 UNAUTHORIZED Unauthorized 
       
       - 402 PAYMENT_REQUIRED Payment Required 
       
       - 403 FORBIDDEN Forbidden 
       
       - 404 NOT_FOUND Not Found 
       
       - 500 INTERNAL_SERVER_ERROR Internal Server Error
       
       - 503 - Service Unavailable
       
____________________________________________________________________________________________________________________________________________________________

   11. What is node.js ?

        Node.js is an open source and cross-platform runtime environment for executing JavaScript code outside of a browser.
        
        NodeJS is not a framework and it’s not a programming language. 
        
        Most of the people are confused and understand it’s a framework or a programming language.
        
        We often use Node.js for building back-end services like APIs like Web App or Mobile App.
        
        It’s used in production by large companies such as Paypal, Uber, Netflix, Walmart and so on.
        
        Node.js is a platform for building the i/o applications which are server-side event-driven and made using JavaScript. 
        
        It is used to build server-side, input-output, event-driven apps. It is built on Google’s V8 engine.
        
___________________________________________________________________________________________________________________________________________________________

   12. Difference between HTTP and HTTPS

       HTTP - HyperText Transfer Protocol (HTTP) is a protocol using which hypertext is transferred over the Web.
       Due to its simplicity, http has been the most widely used protocol for data transfer over the Web but the data 
       (i.e. hypertext) exchanged using http isn’t as secure as we would like it to be. In fact, hyper-text exchanged 
       using http goes as plain text i.e. anyone between the browser and server can read it relatively easy 
       if one intercepts this exchange of data.
       
       HTTPS - https was introduced so that a secure session is setup first between Server and Browser. 
       In fact, cryptographic protocols such as SSL and/or TLS turn http into https i.e. https = http + cryptographic protocols.
       Also, to achieve this security in https, Public Key Infrastructure (PKI) is used because public keys can be used 
       by several Web Browsers while private key can be used by the Web Server of that particular website.
       
       Differences between HTTP and HTTPS

         - HTTP stands for HyperText Transfer Protocol and HTTPS stands for HyperText Transfer Protocol Secure.
         - In HTTP, URL begins with “http://” whereas URL starts with “https://”
         - HTTP uses port number 80 for communication and HTTPS uses 443
         - HTTP is considered to be insecure and HTTPS is secure
         - HTTP Works at Application Layer and HTTPS works at Transport Layer
         - In HTTP, Encryption is absent and Encryption is present in HTTPS as discussed above
         - HTTP does not require any certificates and HTTPS needs SSL Certificates
         - HTTP speed is faster than HTTPS and HTTPS speed is slower than HTTP
         - HTTP does not improve search ranking while HTTPS improves search ranking.
         - HTTP does not use data hashtags to secure data, while HTTPS will have the data before sending it and return it to its original state on the receiver side.

______________________________________________________________________________________________________________________________________________________________________

   13. What are JWT tokens?

       jSON Web Token is an open industry standard used to share information between two entities, 
       usually a client (like your app’s frontend) and a server (your app’s backend). They contain JSON objects 
       which have the information that needs to be shared.

       A JSON web token(JWT) is JSON Object which is used to securely transfer information over the web(between two parties). 
       
       It can be used for an authentication system and can also be used for information exchange.The token is mainly composed of 
       header, payload, signature. These three parts are separated by dots(.). 
       
       JWT defines the structure of information we are sending from one party to the another, and it comes in two forms – Serialized, Deserialized.
       
       

       



  
     

