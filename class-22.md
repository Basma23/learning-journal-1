# REST
**Who is “Roy Fielding”?**

The one who helped write the first web servers, that sent documents across the Internet… and then he did a ton of research explaining why the web works the way it does. His name is on the specification for the protocol that is used to get pages from servers to your browser.

The protocol is capable of all sorts of neat stuff that people ignore for some reason.

**http** tells the browser what protocol to use, and the most important breakthroughs in the history of computing; because it is capable of describing the location of something anywhere in the world from anywhere in the world. It's the foundation of the web. 

The whole world wide web is built on an architectural style called “REST”. REST provides a definition of a “resource”, which is what those things point to.

A web page is a “representation” of a resource. Resources are just concepts. URLs tell the browser that there's a concept somewhere. A browser can then go ask for a specific representation of the concept. Specifically, the browser asks for the web page representation of the concept.

**Representations** is one of these things that doesn't get used a lot. In most cases, a resource has only a single representation. But we're hoping that representations will be used more in the future because there's a bunch of new formats popping up all over the place.

**“Web Services” or "APIs"** means a  machines could use the web. Computers can use those same protocols to send messages back and forth to each other. We've been doing that for a long time but none of the techniques we use today work well when you need to be able to talk to all of the machines in the entire world; because they weren't designed to be used like that. When Fielding and his buddies started building the web, being able to talk to any machine anywhere in the world was a primary concern. Most of the techniques we use at work to get computers to talk to each other didn't have those requirements. You just needed to talk to a small group of machines. So we need some way of having one machine tell another machine about a resource that might be on yet another machine.

On a Web site, redirection is a technique for moving visitors to a different Web page than the one they request, usually because the page requested is unavailable. If everything that machines need to talk about has a corresponding URL, you've created the machine equivalent of a noun. 

Machines don't have a universal noun. Every programming language, database, or other kind of system has a different way of talking about nouns. That's why the URL is so important. It let's all of these systems tell each other about each other's nouns.

 Verbs are important. There's a powerful concept in programming and CS theory called “polymorphism”. That's a geeky way of saying that different nouns can have the same verb applied to them.

GET, can be applied to many different nouns. Some verbs are more specific than others and apply only to a small set of nouns. Some verbs are almost universal like GET, PUT, and DELETE.

HTTP—this protocol Fielding and his friends created—is all about applying verbs to nouns. For instance, when you go to a web page, the browser does an HTTP GET on the URL you type in and back comes a web page.

Web pages usually have images, right? Those are separate resources. The web page just specifies the URLs to the images and the browser goes and does more GETs using the HTTP protocol on them until all the resources are obtained and the web page is displayed. But the important thing here is that very different kinds of nouns can be treated the same. Whether the noun is an image, text, video, an mp3, a slideshow, whatever. I can GET all of those things the same way given a URL.

Every URL would have a human readable and a machine readable representation. When a machine GETs the resource, it will ask for the machine readable one. When a browser GETs a resource for a human, it will ask for the human readable one.

Each of the systems would retrieve information from each other using a simple HTTP GET. If one system needs to add something to another system, it would use an HTTP POST. If a system wants to replace something in another system, it uses an HTTP PUT, or, to do a partial update, it'll hopefully use PATCH. The only thing left to figure out is what the data models should look like.




