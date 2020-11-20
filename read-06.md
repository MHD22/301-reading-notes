##### [back-home](https://mhd22.github.io/301-reading-notes/)

# Read: 06 - Node, Express, and APIs

## What Is Node.js?

* There are plenty of definitions to be found online. 
* Let’s take a look at a couple of the more popular ones. 
* This is what the project’s home page has to say:

 > Node.js® is a JavaScript runtime built on Chrome’s V8 JavaScript engine.

* And this is what Stack Overflow has to offer:

 > Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.


## Node Is Built on Google Chrome’s V8 JavaScript Engine

 The V8 engine is the open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers, including Brave, Opera, and Vivaldi. It was designed with performance in mind and is responsible for compiling JavaScript directly to native machine code that your computer can execute.

#### _____________________________________________


## What Is Node.js Used For?

* Now that we know what Node and npm are and how to install them, we can turn our attention to the first of their common uses: installing (via npm) and running (via Node) various build tools — designed to automate the process of developing a modern JavaScript application.

* These build tools come in all shapes and sizes, and you won’t get far in a modern JavaScript landscape without bumping into them. They can be used for anything from bundling your JavaScript files and dependencies into static assets, to running tests, or automatic code linting and style checking.

#### _____________________________________________

## Are There Any Downsides?

* The fact that Node runs in a single thread does impose some limitations. 
* For example, blocking I/O calls should be avoided, CPU-intensive operations should be handed off to a worker thread, and errors should always be handled correctly for fear of crashing the entire process.

* Some developers also dislike the callback-based style of coding that JavaScript imposes (so much so that there’s even a site dedicated to the horrors of writing asynchronous JavaScript). 
* But with the arrival of native Promises, followed closely by async await, flow control in modern JavaScript has become easier than it ever was.

#### _____________________________________________


## What Are the Advantages of Node.js?

* Aside from speed and scalability, an often-touted advantage of using JavaScript on a web server — as well as in the browser — is that your brain no longer needs to switch modes. 
* You can do everything in the same language, which, as a developer, makes you more productive (and hopefully, happier). 
* For example, you can easily share code between the server and the client.

* Another of Node’s big pluses is that it speaks `JSON`. `JSON` is probably the most important data exchange format on the Web, and the lingua franca for interacting with object databases (such as MongoDB).
* JSON is ideally suited for consumption by a JavaScript program, meaning that when you’re working with Node, data can flow neatly between layers without the need for reformatting. You can have one syntax from browser to server to database.

#### _____________________________________________


## Conclusion

***JavaScript is everywhere, and Node is a vast and expansive subject.***



#### _____________________________________________



### This file wrote by [Mohamad Saad Eddin](https://github.com/MHD22).
***you can visit my profile and follow me.***
### ______________________________________________


###### Thanks for your time, I hope that you have enjoyed.

