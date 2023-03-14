# Path Module

### ***The path module provides utilities for working with file and directory paths.***

```javascript
// Step 1  import module or Require
import path from 'path'
            // or
let path = require('path')

// returns the extension of the path
console.log(path.extname('./app.js'))

// The path.isAbsolute() method determines if path is an absolute path.
console.log(path.isAbsolute('/index.js'))

// The path.join() method joins all given path segments together
console.log(path.join('path','index.js'))

// The path.parse() method returns an object whose properties represent significant elements of the path.
console.log(path.parse('node_module/accepts/index.js'))

// The path.win32 property provides access to Windows-specific implementations of the path methods.
console.log(path.win32)

```