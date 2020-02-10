# Read 05 Undertanding the problem, object literals, DOM

### February 9th, 2020

### _Undertanding the problem domain is the hardest part of programming_
* As every problem in life, if you understand the problem, you already solved 50% of it.
* When we learn something, is important to try to relate it to something that we alerady know, so the new acknowlodge can be better understood.
* When the problem is clear, the solution can be also clear to undertand and to translate to code.
* Is a good technique to divide a problem in parts, and undertand each part, one by one.
* Always the developer should try to have conversations with stakeholders, so he can understand the problem better, and with that undertanding, develop a better product.

### _Object literals_
* An object is composed by properties and methods.
* The value of a property can be string, number, boolean array or another object.
* The value of a method, is always a function.
* Properties are also know as key, and must be uniques on the object.
* In a document, can be _n_ instances of the same object, each one with different name.
* To access an object properties or methods can be by using dot notation pr square brackets. Example:
_var hotelName = hotel.name;_
or
_var roomsName = hotel[name];_

#### Example of an object

var hotel = {    //_curly brackets indicates the start of the object declaration_
  name:'Quay',  //_key/value_
  rooms: 40,    //_key/value_
  booked: 25,   //_key/value_
  checkAvailability: function() {
    return this.room - this.booked;    //function code. "this" is a reference to the object itself.
  }     // _End of function_
};               // _End of object declaration_

### _Document Object Model_
* The DOM is implemented by the browser, creating a model of the page in memory.
* The DOM specifies the way in which the browser should structure the model using a DOM tree, which is made of objects. And each object represents a part of the loaded page.
* APIs lets programs and scripts talk to each other. The DOM states that the script can ask the browser about the current page, and how to tell the browser to update what is been shown to the user.
* The DOM tree consist of four types of nodes: documents nodes, elements nodes, attribute nodes and text nodes.
* Every element, attribute and piece of text in the HTML is represented by is own DOM Node
* An element nodes, could have attributes and text nodes.
* If a DOM query return more than one node, then it will return a nodeList.
