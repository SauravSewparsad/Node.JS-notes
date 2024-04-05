# Node.JS-notes

-------------------------------------------
#Intro to Node.js

History of Node.js
- Node.js, a widely used JavaScript tool, was initially created in 2009 by Ryan Doll.
- Its significant breakthrough in 2011 with the release of npm 1.0 revolutionized code sharing and maintenance.
- The Node.js Foundation, formed in 2015 by IBM, Microsoft, and PayPal, ensures the library's growth and evolution.
-  The community continues to thrive with numerous international conferences and applications.

Introduction to Node.js
- JavaScript, primarily used for front-end development, can be used for a wide range of tasks, including command line tools, server creation, and file system interaction.
- Node.js, adopted by major companies like PayPal, Netflix, and Microsoft, is used for constructing scalable event-driven applications.
- This course covers Node core, standard input, output, module system, and file system.

Javascript and node
- Modern web development uses JavaScript for front-end components, streamlining the process by eliminating syntactical disparities between languages and ensuring consistent functionality across web browsers.
- The author discusses the benefits of code sharing in C# and JavaScript, highlighting the importance of uniformity in coding and data structures.
-  They mention libraries like Underscore, which can be used uniformly on both front-end and back-end, ensuring consistency in user authentication systems and web game development.
-  They also discuss the challenge of maintaining multiple data models with numerous properties across languages, highlighting the importance of minimizing redundancy and maximizing efficiency.
-  By embracing code sharing and unifying the front-end and back-end in a common language, developers can improve maintainability and overall development efficiency.

Pros of javascript 
- Node.js allows code sharing between the back and front ends, with JavaScript's dynamic nature showcasing loose typing.
-  It seamlessly integrates with JSON, a suitable format for web applications. JavaScript simplifies data transfer without complex conversions, making it suitable for various environments.
-  While not a one-size-fits-all solution, sharing JavaScript between front and back ends enhances web app development.

Call backs and asynchronous tasks
- Synchronous processing delays tasks, causing blocking, while asynchronous execution allows for faster progress. Synchronous background processes hinder user interface responsiveness, as seen in applications with grayed-out screens.
- In a computer task completion time ranking, networking, and file system access often require lengthy waits, particularly in web applications. Node's efficiency for web apps stems from its adept handling of such tasks.
- Asynchronous code uses callbacks, like registering a phone number, to execute tasks first, allowing execution to continue and being triggered upon task completion.

----------------------------------------

#Node Global

node global
- creating models
   + Begin by creating a new file in Visual Studio Code, naming it "my-module.js." Simultaneously, initiate another file, "module-demo.js," where the objective is to make the code within "my-module.js" accessible. This exemplifies the potency of code reuse, such as employing a math library across different files or projects.
   + In "my-module.js," utilize the exports object to make data available externally. Create a property named "myText" with a placeholder value - let's say, "hello from module."
   + Node's module loading system is straightforward, maintaining a one-to-one correspondence between files and modules. To access "my-module.js," set its reference to a variable within "module-demo.js" using the require function.
   + For testing purposes, employ a console log to verify that the values retrieved from our module match expectations. Execute the "module-demo.js" file in the console or terminal using the command "node module-demo," and you should observe the console log displaying the "hello from module" placeholder text.

Third party packages
- Node Package Manager (NPM) allows managing packages, including popular third-party modules like Lodash. Install Lodash and navigate to "node_modules" to access its JavaScript files.
- Lodash is installed and creates a file called "demo.js" using the "require" function.
- The "console.log" displays available functions, like "random" for obtaining a random number.
- Nodemon is an example of an NPM package that can be installed globally using the "-g" flag. It executes scripts automatically upon changes, enhancing development efficiency.
-  To track dependencies, the "package.json" file is used to maintain a list of installed packages and their dependencies.

Package.json files
- Create a package.json file to automate package installation for other developers. Node's built-in module for file read and write operations simplifies managing modules and packages.

------------------------------------------------------------------------------------------

#Node modules

node modules
-  Reading from files
    + The text discusses heavy input/output operations, specifically network and disk access, using demo.js as an example and requiring the 'fs' module and library.
    + To read from a temporary JSON file, create an object with a property named 'name' and use the'readFile' function to access the file system. Alternatively, use an anonymous function or a concise arrow 
      function.
    + The execution encounters an unexpected output due to the absence of a specified file format. To resolve this, the callback is moved to the third parameter and 'UTF-8' is added.
    + An alternative method involves accessing the JSON file using 'require' directly. By creating a 'data' variable and setting it to 'require' with the path to data.json, we can log the data. Now, we 
      observe two distinct objects in our console - one from 'require' and another from 'readFile.'
    + The'require' object is a true object, while the'readFile' object is a string. To resolve this, a new variable 'data' is created and converted to JSON.

Directory access
- Explore directory reading by using the 'fs' module and'readdir' function to access the file system, specifying the directory location to read, like Drive C.
- Establish a callback, log data, save changes, execute demo with nodemon, and observe output for all directories in Drive C, illustrating the simple process of reading directories.

Writing to Files
- The text focuses on file writing, starting with file creation and using the writeFile function. The file name is passed as the first parameter, and the data is defined as a JSON object with a name of 'Bob'.
- The script node demo.js generates a data.json file, but the content doesn't match expectations. To fix this, we convert the object to a string using JSON.stringify, resulting in the desired JSON format.
- The script functions correctly, but a deprecation warning warns against calling an asynchronous function without a callback. A callback function is created, eliminating the warning and providing feedback.
------------------------------------------------------------

#Node file management and streams

Node framework
- what a framework is. In simple terms, it serves as a foundational structure, much like the support structure of a building or vehicle. In software development, a framework provides the essential structure that allows developers to build upon it.
- Web frameworks are essential for web development, particularly for creating large APIs or HTTP servers.
- They provide a structured foundation for tasks like serving static files or constructing web APIs.
- Popular Node.js frameworks include Express, Sails, and Koa. Express is known for its simplicity, while Sails is a feature-rich framework with additional functionalities.
- Koa is a modern framework with innovative features.

Express
- Express.js is a web framework designed for Node, supporting web applications and web APIs. Web applications are functionalities running on browsers or mobile devices, often communicating with servers for tasks like user authentication or data retrieval.
- Express.js, a Node-based web app, enables communication with the back end of platforms like Twitter, despite its back-end nature. Its extensive community support and online documentation make it a valuable addition to the overall app.

Socket.io
- Socket.io offers real-time, two-way event-driven communication, addressing Express's limitation.
- It combines a client-side library for browsers and a server-side library for Node.js, both with similar APIs.
- The mechanism will be explored in a demonstration application.
--------------------------------
#Modual summary

Moduale summary
We created a robust chat application using Node.js, Socket.IO, and MongoDb-powered mLab. We explored synchronous and asynchronous code, handling tasks like callbacks, promises, and async/await. We embraced test-driven development, and if satisfied, explore with React or Angular frameworks.
