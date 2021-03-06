#javascript-obfuscator plugin for Webpack

[![npm version](https://badge.fury.io/js/webpack-obfuscator.svg)](https://badge.fury.io/js/webpack-obfuscator)

### Installation

Install the package with NPM and add it to your devDependencies:

`npm install --save-dev webpack-obfuscator`

### Usage:

```javascript
var WebpackObfuscator = require('webpack-obfuscator');

// ...

// webpack plugins array
plugins: [
	new WebpackObfuscator({
      rotateUnicodeArray: true
  }, ['excluded_bundle_name.js'])
],
```

### obfuscatorOptions
Type: `Object` Default: `null`

Options for [javascript-obfuscator](https://github.com/sanex3339/javascript-obfuscator). Should be passed exactly like described on their page.

### excludes
Type: `Array` or `String` Default: `[]`

Examples: `['excluded_bundle_name.js', '**_bundle_name.js']` or `'excluded_bundle_name.js'`

Can be used to bypass obfuscation of some files.

### License
Copyright (C) 2016 [Timofey Kachalov](http://github.com/sanex3339).

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

  * Redistributions of source code must retain the above copyright
    notice, this list of conditions and the following disclaimer.
  * Redistributions in binary form must reproduce the above copyright
    notice, this list of conditions and the following disclaimer in the
    documentation and/or other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
ARE DISCLAIMED. IN NO EVENT SHALL <COPYRIGHT HOLDER> BE LIABLE FOR ANY
DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF
THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.