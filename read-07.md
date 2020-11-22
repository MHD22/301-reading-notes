##### [back-home](https://mhd22.github.io/301-reading-notes/)

# Read: 07 - APIs continued

## Who is “Roy Fielding”?

* The man which helped write the first web servers, that sent documents across the Internet… and then he did a ton of research explaining why the web works the way it does. 
* His name is on the specification for the protocol that is used to get pages from servers to your browser.

#### _____________________________________________

## how do the machines tell each other where things are?

* The URL, of course. If everything that machines need to talk about has a corresponding URL, you've created the machine equivalent of a noun. 
* That you and I and the rest of the world have agreed on talking about nouns in a certain way is pretty important

* Machines don't have a universal noun - that's why they suck. Every programming language, database, or other kind of system has a different way of talking about nouns. That's why the URL is so important. It let's all of these systems tell each other about each other's nouns.

* HTTP—this protocol Fielding and his friends created—is all about applying verbs to nouns. For instance, when you go to a web page, the browser does an HTTP GET on the URL you type in and back comes a web page.

* Web pages usually have images, right? Those are separate resources. The web page just specifies the URLs to the images and the browser goes and does more GETs using the HTTP protocol on them until all the resources are obtained and the web page is displayed. But the important thing here is that very different kinds of nouns can be treated the same. Whether the noun is an image, text, video, an mp3, a slideshow, whatever. I can GET all of those things the same way given a URL.

#### _____________________________________________

##  How about we take a real example.

* Imagine you are a teacher - at school you probably have a big computer system, or three or four computer systems more likely, that would let you manage students: what classes they're in, what grades they're getting, emergency contacts, information about the books you teach out of, etc. 
* If the systems are web-based, then there's probably a URL for each of the nouns involved here: student, teacher, class, book, room, etc. Right now, getting the URL through the browser gives you a web page. If there were a machine readable representation for each URL, then it would be trivial to latch new tools onto the system because all of that information would be consumable in a standard way. 
* It would also make it quite a bit easier for each of the systems to talk to each other. Or, you could build a state or country-wide system that was able to talk to each of the individual school systems to collect testing scores. The possibilities are endless.


* Each of the systems would retrieve information from each other using a simple HTTP GET. 
* If one system needs to add something to another system, it would use an HTTP POST. 
* If a system wants to replace something in another system, it uses an HTTP PUT,
* or, to do a partial update, it'll hopefully use PATCH. 
* The only thing left to figure out is what the data models should look like.





#### _____________________________________________



### This file wrote by [Mohamad Saad Eddin](https://github.com/MHD22).
***you can visit my profile and follow me.***
### ______________________________________________


###### Thanks for your time, I hope that you have enjoyed.

