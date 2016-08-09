# V3ctor JavaScript Sdk #

## Description ##
V3ctor WareHouse JavaScript Sdk.

## Requirements ##
* [JQuery](https://jquery.com/)

## Developer Documentation ##
JsDoc.

## Installation ##
Add Jquery to HTML Document.

~~~

<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.0/jquery.min.js"></script>

~~~

Add V3SDK.js to HTML Document.

~~~

<script src="V3SDK.js"></script>

~~~

## Example ##
~~~

v3 = new V3SDK("https://v3-yorch.rhcloud.com/", "lYltuNtYYbYRFC7QWwHn9b5aH2UJMk1234567890");

v3obj = {client: "V3ctor Js SDK", message: "Hello World"};

// New Object
v3.newObject("jsdk", v3obj, function(data){
  console.log(data);
  
  console.log(V3SDK.getId(data));
});

var id = "57a9f2e4409b60347e8b4567";

// Find by Id
v3.findObject("jsdk", id, function(data){
  console.log(data);
});

var v3Query = {message: "Hello World"};

// Query
v3.query("jsdk", v3Query, function(data){
  console.log(data);
});

v3obj = {msg: "msg updated"};

// Update Object by Id
v3.updateObject("jsdk", id, v3obj, function(data){
  console.log(data);
});

// Delete Object
v3.deleteObject("jsdk", id, function(data){
  console.log(data);
});

~~~

## References ##
https://en.wikipedia.org/wiki/JSONP

P.D. Let's go play !!!







