# Forms
The best known form on the web is probably the search box that sits right in the middle of Google's homepage.
A user fills in a form and then presses a button to submit the information to the server.
- There are several types of form controls :
1. ADDING TEXT
2. Making Choices:
3. Submitting Forms:
4. Uploading Files:
## Form Structure
```
<form action="http://www.example.com/subscribe.php"
method="get">
<p>This is where the form controls will appear.
 </p></form>
 ```
 

>  Whenever you want to collect information from visitors you will need a form, which lives inside a ```<form>``` element.

> Information from a form is sent in name/value pairs.

> Each form control is given a name, and the text the user types in or the values of the options they select are sent to the server.

> HTML5 introduces new form elements which make it easier for visitors to fill in forms.

# Lists, Tablesand Forms

In addition to the CSS properties covered in other chapters which work with the contents of all elements,
there are several others that are specifically used to control the appearance of lists, tables, and forms.
 List markers can be given different appearances using the list-style-type and list-style image
properties. 
Table cells can have different borders and spacing in different browsers, but there are properties you can use to control them and make them more consistent.
 Forms are easier to use if the form controls are vertically aligned using CSS. 
Forms benefit from styles that make them feel more interactive.
# EVENTS
When you browse the web, your browser registers different types of events. It's the browser's way of saying, "Hey, this
just happened." Your script can then respond to these events. 

## DIFFERENT EVENT TYPES 
- load :  Web page has finished loading 
- unload :  Web page is unloading (usually because a new page was requested) 
- error :  Browser encounters a JavaScript error or an asset doesn't exist 
- resize :  Browser window has been resized
- scroll :  User has scrolled up or down the page 
# TERMINOLOGY 
> EVENTS TRIGGER SCRIPTS
Events are said to trigger a function or script. When the click event fires on the element in this diagram, it could trigger a script that enlarges
the selected item. 
# HOW EVENTS TRIGGER JAVASCRIPT CODE 
1. Select t he element node(s) you want the script to respond to. 
2. Indicate which event on the selected node(s) will trigger the response.
Programmers call this binding an event to a DOM node. 
3. State the code you want to run when the event occurs. 

Events are the browser's way of indicating when something has happened (such as when a page has
finished loading or a button has been clicked).

Binding is the process of stating which event you are waiting to happen, and which element you are waiting
for that event to happen upon. When an event occurs on an element, it can trigger a JavaScript function. When this function then changes
the web page in some way, it feels interactive because it has responded to the user.

You can use event delegation to monitor for events that happen on all of the children of an element.

The most commonly used events are W3C DOM events, although there are others in the HTMLS specification as well as browser-specific events.


