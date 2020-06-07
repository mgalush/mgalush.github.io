# Questions

1. **Why would you want to run JavaScript code outside of a browser?**
You can write JS outside of a browser using Node.js.  Reasons for doing this are when you want to write code that interacts with the backend, such as when you are accessing a database or calling an API.  Other reasons may be that you don't want the code visible to the user, such as for security reasons, or that you would like your code to continue executing once you have closed the browser, such as when placing an order online. 

2. **What is the difference between a module and a package?**
A *package* is a file or directory.  The contents of that file or directory are found in the package.json file that accompanies the file.  A *module* is a file or directory that can be loaded using Node.js.  If a package contains a pack.json file, it is also a module. 

3. **What does the node package manager do?**
NPM is a package manager which allows you to download various Node.js modules/packages to include in your file.

4. **Provide code snippets showing 3 different ways to export a function from a node module**
You use `module.exports` to export from a node module.

Exporting a single function:
```
// helpers.js
module.exports = function(x) {
  return x * 2
}

// index.js
const helpers = require('./helpers.js')
helpers(4) // => 8
```

Exporting several functions:
```
// helpers.js
module.exports = {
  multiplyByTwo: function(x) { return x *2 },
  divideByTwo: function(x) { return x / 2}
}

// index.js
const helpers = require('./helpers.js')
helpers.multiplyByTwo(10) // => 5
```

Exporting objects:
```
// assigning named exports
module.exports.pizza = true
exports.pizza = true

// exporting an object
module.exports = {}
exports = {}
```

# Vocabulary

* Ecosystem: a system or network of interconnecting and interacting parts
* Node.js: a server-side platform for easily building fast and scalable network applications 
* V8 Engine: Google's open source JavaScript and WebAssembly engine
* Module: a file or directory loaded by node.js
* Package: a file or directory used by npm to run code in node.js
* NPM: a package manager for node.js which allows developers to easily share and borrow packages
* Server: a computer or device that provides a service to another computer program and its user (the client)
* Environment: the state of a computer, determined by a combination of software and hardware
* Interpreter: a program that reads code and executes instructions
* Compiler: a program that reads code and translates the code into machine code


### Sources

* [NPM Documentation](https://docs.npmjs.com/)
* [Node Exports Medium Article](https://medium.com/@osiolabs/use-module-exports-to-keep-node-js-code-organized-9379526ebac8)
* [Ecosystem](https://www.dictionary.com/browse/ecosystem#:~:text=noun%20Ecology.,depends%20on%20hardware%2Fsoftware%20integration.)
* [Node.js](https://www.tutorialspoint.com/nodejs/nodejs_introduction.htm)
* [V8 Engine](https://v8.dev/)
* [Server](https://whatis.techtarget.com/definition/server)
* [Environment](https://www.webopedia.com/TERM/E/environment.html#:~:text=environment,basic%20hardware%20and%20software%20characteristics.&text=(2)%20In%20DOS%20systems%2C,various%20types%20of%20miscellaneous%20information.)
* [Interpeter and Compiler](https://medium.com/hackernoon/compilers-and-interpreters-3e354a2e41cf#:~:text=Compiler%20vs.&text=The%20main%20difference%20is%20that,representation%20and%20immediately%20evaluate%20it.)
