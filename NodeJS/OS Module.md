# OS Module

###  ***The os module provides operating system-related utility methods and properties.***

```javascript
// import OS module
const os=require('os')
// Returns the operating system CPU architecture
console.log(os.arch())
// Returns an array of objects containing information about each logical CPU core.
console.log(os.cpus())
// Returns the amount of free system memory in bytes as an integer.
console.log(os.freemem())
// Returns the string path of the current user's home directory.
console.log(os.homedir())
// Returns an object containing network interfaces that have been assigned a network address.
console.log(os.networkInterfaces())
// Returns the total amount of system memory in bytes as an integer.
console.log(os.totalmem())
// Returns a string identifying the operating system
console.log(os.platform())
// Returns the host name of the operating system as a string.
console.log(os.hostname())
```