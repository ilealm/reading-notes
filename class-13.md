# Read 13 The Past, Present, and Future of Local Storage for Web Applications

### February 18th, 2020


### _Local storage_
* Persistent local storage, may be stored in the registry, INI files, XML files, or some other place according to platform convention.
* Cookies where designed to be a local storage of small amounts of data.

  _Things to consider when using cookies..._
  * Slowing down your web application by needlessly transmitting the same data over and over.
  * Sending data unencrypted over the internet (unless your entire web application is served over SSL)
  * Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.

* For local storage, we need:
  * A lot of storage space
  * On the client side
  * That persists beyond a page refresh
  * And isn’t transmitted to the server

### _HTML Local Stotage_
  * It’s a way for web pages to store named key/value pairs locally, within the client web browser.
  * This data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. 
  * Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually). 
  * Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.

####  _Accesing HTML5 Local Storage_
  * From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object. Before you can use it, you should detect whether the browser supports it.
  * To keep track programmatically of when the storage area changes, you can trap the storage event.