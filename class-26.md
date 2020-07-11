# EJS
**EJS** is a simple templating language that lets you generate HTML markup with plain JavaScript. No religiousness about how to organize things. No reinvention of iteration and control-flow. It's just plain JavaScript.
- Use plain JavaScript
- Fast development time
- Simple syntax
- Speedy execution
- Easy debugging
- Active development

**Features**
- Fast compilation and rendering
- Simple template tags: ```<% %>```
- Custom delimiters (e.g., use ```[? ?]``` instead of ```<% %>```)
- Sub-template includes
- Ships with CLI
- Both server JS and browser support
- Static caching of intermediate JavaScript
- Static caching of templates
- Complies with the Express view system

**Use EJS to Template Your Node Application**
When creating quick on-the-fly Node applications, an easy and fast way to template our application is sometimes necessary. So far we've been building out full MEAN applications and Angular acts as our templating engine.

For applications that need quick templating, there are many options that we can use. Jade comes as the view engine for Express by default but that syntax just flat out scares me. EJS is one alternative does that job well and is very easy to set up. 

EJS let's us spin up quick applications when we don't need anything too complex. By using partials and having the ability to easily pass variables to our views, we can build some great applications quickly.