## Sencha Touch and Ext JS adaptor for Sinon.JS

**sinon-sencha** is a tiny adaptor that tweaks [Sinon.JS](http://sinonjs.org/)'s format() method to make it aware of the Sencha Touch and Ext JS class system.

Without this adaptor, Sinon will treat Sencha Touch and Ext JS class instances as deeply nested Objects and attempt to recursively traverse and format all of their instance properties.  This produces unnecessarily verbose assertion messages that will cause tests to run very slowly.

## Installation and Usage

### &lt;script&gt; tag:

First, include `ext.js` (or `ext-all.js`, etc.) and `sinon.js` in your HTML test runner:


	<script src="ext.js"></script>
	<script src="sinon.js"></script>

Then reference `sinon-sencha.js`:
	
	<script src="sinon-sencha.js"></script>

or, if you prefer the minified version:

	<script src="sinon-sencha.min.js"></script>

### Karma Test Runner

Reference `sinon-sencha.js` or `sinon-sencha.min.js` in the `files` section of your `karma.conf.js` file.

**NOTE:** Be sure to reference `sinon-sencha.js` *after* including both `ext.js` (or `ext-all.js`, etc.) and `sinon.js`.

## Contributors

* [John Yanarella](http://twitter.com/johnyanarella) (Creator)

## License

Copyright (c) 2013 [CodeCatalyst, LLC](http://www.codecatalyst.com/)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.