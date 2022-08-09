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
  
     

