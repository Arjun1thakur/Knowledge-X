# FS Module
* ***The fs module enables interacting with the file system***
* ***All file system operations have synchronous, callback, and promise-based forms, and are accessible using both CommonJS syntax and ES6 Modules (ESM).***

## Promise Example
***Promise-based operations return a promise that is fulfilled when the asynchronous operation is complete.***

```javascript
// Normal
const { unlink } = require('fs/promises');

(async function(path) {
  try {
    await unlink(path);
    console.log(`successfully deleted ${path}`);
  } catch (error) {
    console.error('there was an error:', error.message);
  }
})('/tmp/hello');

            // or
// ES6
import { unlink } from 'fs/promises';

try {
  await unlink('/tmp/hello');
  console.log('successfully deleted /tmp/hello');
} catch (error) {
  console.error('there was an error:', error.message);
}
```

## Callback Example
***The callback form takes a completion callback function as its last argument and invokes the operation asynchronously.***
```javascript
const { unlink } = require('fs');

unlink('/tmp/hello', (err) => {
  if (err) throw err;
  console.log('successfully deleted /tmp/hello');
});
```

## Synchronous example
***The synchronous APIs perform all operations synchronously, blocking the event loop until the operation completes or fails.***

```javascript
import { unlinkSync } from 'fs';
try {
  unlinkSync('/tmp/hello');
  console.log('successfully deleted /tmp/hello');
} catch (err) {
  // handle the error
}
```
## ```file system Sync```

```javascript
// Import file system module
const fs = require('fs')
// Create directory or folder
fs.mkdirSync('test')
// Create file with some text
fs.writeFileSync('test/test.txt','my name is arjun')
// Read file 
const data=fs.readFileSync('test/test.txt',"utf8")
// Rename file
fs.renameSync('Test.txt','demo.txt')
// Delete file
fs.unlinkSync('demo.txt')
// Delete folder
fs.rmdirSync('test')
```

## ```file system Async```
```javascript
// Import file system module
const fs = require('fs')
// Create directory or folder
fs.mkdir('test',()=>{
    console.log('ok')
})
// Create file with some text
fs.writeFile('test/demo.txt','try demo',(error)=>{
    console.log(error)
})
// Read file 
fs.readFile('test/demo.txt',(error,data)=>{
    console.log(data.toString())
})
// Rename file
fs.unlink('test/demo.txt',(error)=>{
    console.log(error)
})
// Delete file
fs.rmdir('test',(error)=>{
    console.log(error)
})
```