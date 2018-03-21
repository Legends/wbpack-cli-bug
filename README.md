# wbpack-cli-bug


Clone the repo.

npm install

npm run build   --> webpack ./hello.js hello.bundle.js

You get:
ERROR in multi ./hello.js hello.bundle.js
Module not found: Error: Can't resolve 'hello.bundle.js'


Now, when you do:
webpack ./hello.js -o hello.bundle.js

This will generate a `hello.bundle.js`.


Now when you execute:

webpack ./hello.js hello.bundle.js  (again as the first time without -o flag)

It will work. But it will not work if the output bundle does not already exist!
