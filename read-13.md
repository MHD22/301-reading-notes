##### [back-home](https://mhd22.github.io/301-reading-notes/)


# Read: 13 - Update/Delete


* ***An HTML form on a web page is nothing more than a convenient user-friendly way to configure an HTTP request to send data to a server.*** 
* ***This enables the user to provide information to be delivered in the HTTP request.***

#### _____________________________________________

## On the client side: defining how to send the data

* The `<form>` element defines how the data will be sent. 
* All of its attributes are designed to let you configure the request to be sent when a user hits a submit button. 
* The two most important attributes are action and method.

### The action attribute:

* The action attribute defines where the data gets sent. 
* Its value must be a valid relative or absolute URL. 
* If this attribute isn't provided, the data will be sent to the URL of the page containing the form — the current page.

`<form action="https://example.com">`


### The method attribute:

* The method attribute defines how data is sent. 
* The HTTP protocol provides several ways to perform a request; HTML form data can be transmitted via a number of different methods, the most common being the `GET` method and the `POST` method.

#### _____________________________________________

## On the server side: retrieving the data:

* Whichever HTTP method you choose, the server receives a string that will be parsed in order to get the data as a list of key/value pairs.
* The way you access this list depends on the development platform you use and on any specific frameworks you may be using with it.

#### _____________________________________________

## Summary:

sending form data is easy, but securing an application can be tricky. Just remember that a front-end developer is not the one who should define the security model of the data.It's possible to perform client-side form validation, but the server can't trust this validation because it has no way to truly know what has really happened on the client-side.

#### _____________________________________________



### This file wrote by [Mohamad Saad Eddin](https://github.com/MHD22).
***you can visit my profile and follow me.***
### ______________________________________________


###### Thanks for your time, I hope that you have enjoyed.