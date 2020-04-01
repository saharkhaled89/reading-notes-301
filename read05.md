# Heroku: Getting Started with Node

* Set up

* Prepare the app

* Deploy the app

* View logs

* Define a Procfile :Use a Procfile, a text file in the root directory of your application, to explicitly declare what command should be executed to start your app.

* Scale the app

* Declare app dependencies
Heroku recognizes an app as Node.js by the existence of a package.json file in the root directory. For your own apps, you can create one by running npm init --yes.

* Run the app locally
Now start your application locally using the heroku local command, which was installed as part of the Heroku CLI:

**$heroku local web**

**[OKAY] Loaded ENV .env File as KEY=VALUE Format**

**1:23:15 PM web.1 |  Node app is running on port 5000**

**Just like Heroku, heroku local examines the Procfile to determine what to run.**

* Push local changes
In this step you’ll learn how to propagate a local change to the application through to Heroku. As an example, you’ll modify the application to add an additional dependency and the code to use it.

* Provision add-ons
Add-ons are third-party cloud services that provide out-of-the-box additional services for your application, from persistence through logging to monitoring and more.

* Start a console
Define config vars
Heroku lets you externalize configuration - storing data such as encryption keys or external resource addresses in config vars.

# Deploying a Simple Blog to Heroku

**Error pages are not what typically appear on your screen when you're surfing the web, but when it happens it's so annoying! To see how servers work from within, we will build a simple web server by ourselves. We will use Node.js as a server part technology for that task. Then we'll use Heroku cloud application platform to turn this local server into a world wide server.**

**We will use Node.js for our project. Node.js is an open source, cross-platform runtime environment, which allows you to build server-side and networking applications. It's written in JavaScript and can be run within the Node.js runtime on any platform.**

