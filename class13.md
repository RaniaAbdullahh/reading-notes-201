# LOCAL STORAGE FOR WEB APPLICATIONS
web applications have  three potentially dealbreaking downsides:
1. Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
2. Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
3. Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful
## HTML5 STORAGE
it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you.
> From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object. Before you can use it, you should detect whether the browser supports it.

- you can use Modernizr to detect support for HTML5 Storage.

```
if (Modernizr.localstorage) {
  // window.localStorage is available!
} else {}
```
## USING HTML5 STORAGE
- HTML5 Storage is based on named key/value pairs.
- You store data based on a named key, then you can retrieve that data with the same key. 
-  The named key is a string.
- The data can be any type supported by JavaScript.
- the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.
- you can treat the localStorage object as an associative array. Instead of using the getItem() and setItem() methods, you can simply use square brackets:
```
var foo = localStorage.getItem("bar");
// ...
localStorage.setItem("bar", foo);
```
- there is a property to get the total number of values in the storage area, and to iterate through all of the keys by index (to get the name of each key)
```
interface Storage {
  readonly attribute unsigned long length;
  getter DOMString key(in unsigned long index);
};
```
**If you call key() with an index that is not between 0–(length-1), the function will return null.**
## TRACKING CHANGES TO THE HTML5 STORAGE AREA
The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something. For example, if you set an item to its existing value or call clear() when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.
```
f (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};
```
## LIMITATIONS IN CURRENT BROWSERS
> “5 megabytes” is how much storage space each origin gets by default. This is surprisingly consistent across browsers, although it is phrased as no more than a suggestion in the HTML5 Storage specification. One thing to keep in mind is that you’re storing strings,
At time of writing (February 2011), no browser supports any mechanism for web developers to request more storage space. Some browsers (like Opera) allow the user to control each site’s storage quota, but it is purely a user-initiated action, not something that you as a web developer can build into your web application.
## BEYOND NAMED KEY-VALUE PAIRS: COMPETING VISIONS
> One vision is an acronym that you probably know already: SQL. In 2007, Google launched Gears, an open source cross-browser plugin which included an embedded database based on SQLite. This early prototype later influenced the creation of the Web SQL Database specification. Web SQL Database (formerly known as “WebDB”) provides a thin wrapper around a SQL database, allowing you to do things like this from JavaScript:
