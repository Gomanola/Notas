// npm - global command, comes with node

// yarn - alternative to npm

  

// npm --version

// yarn --version

  

// local dependency - use it only in this particular project

// npm i <packageName>

  

// global dependency - use it in any project

// npm install -g <packageName>

  

// package.json - manifest file (stores important info about project/package)

// manual approach (create package.json in the root, create properties etc)

// npm init (step by step, press enter to skip)

// npm init -y (everything default)

  
  

// yarn init -y

// yarn add <packageName> (npm i <packageName>)

// yarn global add <packageName> (npm install -g <packageName>)

  

// npm uninstall <packageName>

// yarn remove <packageName>

  

// npm update <packageName>

// yarn upgrade <packageName>

  

// npm -v

// node -v

// npm init -y

// npm install bootstrap

// npm install lodash

// npm uninstall bootstrap

// npm update lodash

// npm install bootstrap@5.3.8

// npm install lodash@4.18.1

  

// npm i nodemon -D

// yarn add nodemon -D

  

const _ = require('lodash')

  

const items = [1, [2, [3, [4]]]]

console.log('Hello world');

const newItems = _.flattenDeep(items)

console.log(newItems);