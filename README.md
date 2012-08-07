node-json2xml
===========

Description
-----------

Simple JavaScript Object to XML string converter.

Installation
------------

Simplest way to install `json2xml` is to use [npm](http://npmjs.org), just `npm
install json2xml` which will download json2xml and all dependencies.

Simple usage
-----------
    
    var json2xml = require('json2xml');
    json2xml({a:1});
    //<a>1</a>
	    

Options
-----------

	add header:

	json2xml({a:1}, { header:true });
	//<?xml version="1.0" encoding="UTF-8"?><a>1</a>

	add node attributes:

	json2xml({a:1, attr:{b:2,c:3 }}, { attributes_key:'attr' });	
	// <a b="2" c="3" >1</a>