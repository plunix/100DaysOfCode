# 100 Days of Code Challenge : Day 2: Babel
<small>**Date:** <i>Tuesday, June 26, 2018</i></small>

## Overview
Babel is a code transpiler that allows developers to write ECMAScript2015+ (i.e. ES6+) Javascript code.  Babel will take your Javascript code and compile it down to code that can be read by older browsers that are not yet able to read newer Javascript APIs that are made available by ECMAScript2015+ (e.g. module imports using the "import" syntax, Javascript classes, etc.)

## Instructions
1. **Run** ```yarn add``` or ```npm install```
2. **Run** ```yarn runnode```
    
    Result: Console should log an error because node does not yet support ES6+ syntax.
3. **Run** ```yarn runbabel```
    
    Result: Console should successfully execute the code.
## Gotchas

1. **Babel requires the following to function properly:**

    ### Packages
    1. **babel-cli**
    2. **babel-preset-env**
    ### Files 
    1. **.babelrc** (or babel configuration object in your pacakage.json)
2. **To execute your code via the command line as you would with the "node" command"**:
    
    1. Install "**@babel/core** and **@babel/node**" in your project's dev dependencies by running ```yarn add --dev @babel/core @babel/node```
    2. Run ```babel-node [yourfilename].js```

    <small>**Note**: While you can install @babel/core and @babel/node as actual dependecies, it's better to make them dev dependecies so that these libraries are not installed in your production environment.</small>

## References
- [Babel JS] (https://babeljs.io/docs/en/index.html)