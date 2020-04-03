# What Is Node and When Should I Use It?

**Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.**

# Node Is Built on Google Chrome’s V8 JavaScript Engine

*The V8 engine is the open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers, including Brave, Opera, and Vivaldi. It was designed with performance in mind and is responsible for compiling JavaScript directly to native machine code that your computer can execute.*

*Node.js is a program we can use to execute JavaScript on our computers. In other words, it’s a JavaScript runtime.*

# How Do I Install Node.js?

## Node Binaries vs Version Manager

*Many websites will recommend that you head to the official Node download page and grab the Node binaries for your system. While that works, I would suggest that you use a version manager instead. This is a program that allows you to install multiple versions of Node and switch between them at will.*

**The advantages of using a version manager:**

* it negates potential permission issues when using Node with npm and lets you set a Node version on a per-project basis.

# Introducing npm, the JavaScript Package Manager

* Node comes bundled with a package manager called npm. To check which version you have installed on your system, type npm -v.

* In addition to being the package manager for JavaScript, npm is also the world’s largest software registry. 

# Installing a Package Globally

* npm install -g jshint: This will install the jshint package globally on your system. We can use it to lint the index.js for example:jshint index.js.

# Installing a Package Locally

* npm init -y: This will create and auto-populate a package.json file in the same folder.

* npm install lodash --save:use npm to install the lodash package and save it as a project dependency.

# Working with the package.json File

**node_modules. This is where npm has saved lodash and any libraries that lodash depends on. The node_modules folder shouldn’t be checked in to version control, and can, in fact, be re-created at any time by running npm install from within the project’s root.**

**If you open the package.json file, you’ll see lodash listed under the dependencies field. By specifying your project’s dependencies in this way, you allow any developer anywhere to clone your project and use npm to install whatever packages it needs to run.**


# What Is Node.js Used For?

*  developing apps with any modern JavaScript framework (for example, React or Angular), you’ll be expected to have a working knowledge of Node and npm (or maybe Yarn).

* these frameworks (and many, many related packages) are all available via npm and rely on Node to create a sensible development environment in which they can run.

# The Node.js Execution Model

![img](/img/ec.png)

# What Kind of Apps Is Node.js Suited To?

*Node is particularly suited to building applications that require some form of real-time interaction or collaboration — for example, chat sites, or apps such as CodeShare, where you can watch a document being edited live by someone else. It’s also a good fit for building APIs where you’re handling lots of requests that are I/O driven (such as those needing to perform operations on a database), or for sites involving data streaming, as Node makes it possible to process files while they’re still being uploaded.*

# What Are the Advantages of Node.js?

*  Node’s big pluses is that it speaks JSON. JSON is probably the most important data exchange format on the Web, and the lingua franca for interacting with object databases (such as MongoDB). JSON is ideally suited for consumption by a JavaScript program, meaning that when you’re working with Node, data can flow neatly between layers without the need for reformatting. You can have one syntax from browser to server to database.

* JavaScript is ubiquitous: most of us are familiar with JavaScript, or have used it at some point. This means that transitioning to Node development is potentially easier than to other server-side languages. 

     **JavaScript is everywhere, and Node is a vast and expansive subject** 