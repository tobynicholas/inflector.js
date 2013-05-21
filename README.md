Inflector.js
============

This code is based in part on the work done in Ruby to support inflection as part of Ruby on Rails in the ActiveSupport Inflector and Inflections classes.  It was initally ported to Javascript by Ryan Schuft (ryan.schuft@gmail.com) in 2007.

This version has been adapted by Toby Marsden from Inflection-JS available at http://code.google.com/p/inflection-js/. The aim is to provide inflections missing from Ember.String. 

The basic usage is:

1. Include this script on your web page after Ember.js
2. Call functions on any String object in Javascript

If the Ember.EXTEND\_PROTOTYPES flag has been set to false, the String prototypes will not be extended, and you will need to  instead call the function on `Inflector.String`, e.g. `Inflector.String.titleize("message_properties")`

Currently implemented functions:

	String.pluralize(plural) == String
- renders a singular English language noun into its plural form
- normal results can be overridden by passing in an alternative

	String.singularize(singular) == String
- renders a plural English language noun into its singular form 
- normal results can be overridden by passing in an alterative

	String.humanize(lowFirstLetter) == String
- renders a lower case and underscored word into human readable form
- defaults to making the first letter capitalized unless you pass true

	String.titleize() == String
- renders words into title casing (as for book titles)

	String.tableize() == String
- renders camel cased singular words into their underscored plural form

Copyright (c) 2010 Ryan Schuft (ryan.schuft@gmail.com)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
