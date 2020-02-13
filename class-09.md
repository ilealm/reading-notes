# Read 09 Forms and Events

### February 12th, 2020


### _Forms_
* Form controls enable collect dara form users.
* Common form controls:
  * To add text:
    * Text input,
    * Password input,
    * Text area
  * Making choices
    * Radio button
    * Checkboxes
    * Drop-down boxes
  * Submiting forms
    * Submmiting buttons
    * Image buttons
  * Uploading files
    * File upload
    * Image buttons
  * Uploading files
    * File upload
  * When the user submit the page, each control is sent to the server along with its values, which returns a new page to send back.
  * Form controls live inside the form element. 
  * The action attribute of the form is the URL of the page on the server which will receive the information when the page is submited.
  * Forms can have a method either post ot get.
    * get: the values of the controls will be attached in the URL for the action page.
    * post: form values are sended as HTPP headers. Use this method for upload files, long forms, sensitive data, adds/deletes information fo a data base.
  * Each control must contain a unique name in the form.


### _CSS_
* The apperiance of a list can be changed by list-style-type.
* The possition of the marker of a list can be unpaded by list-syle-position property.
* Examples of table formating:
  * width, padding, text-transform, letter-spacing, border, background-color, hover, align numerals, shade alternative rows, border-spacing, border-collapse.

### _Events_
* Events can exist with interactions from the users or other devices.
* Examples of events: 
  * focus, blur, input, change, submit, paste, select, click, load, scroll...
* Java event handling when a event is trigged:
  1. Selelct the element node  you want the script to respond.
  1. Indicate which event on the selected node(s) will trigger the response.
  1. State the code you want to run when the event occurs.
* JavaScript allow to responde to events.
* Event listeners are able to perfom more than one function at the time. Not supported in all browsers.