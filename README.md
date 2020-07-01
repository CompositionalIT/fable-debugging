# Fable Minimal App

This is a small Fable app project so you can easily get started and add your own code easily in it.

## Requirements

* [dotnet SDK](https://www.microsoft.com/net/download/core) 3.0 or higher
* [node.js](https://nodejs.org) with [npm](https://www.npmjs.com/)
* An F# editor like Visual Studio, Visual Studio Code with [Ionide](http://ionide.io/) or [JetBrains Rider](https://www.jetbrains.com/rider/).

## Building and running the app

* Install JS dependencies: `npm install`
* In VS Code: F5
  * Calls `npm run start`
  * Launches the app
  * Attaches the VS Code debugger to Chrome

### Debug Console in VS Code
Debug output is shown directly in VS Code:
![image](https://user-images.githubusercontent.com/1781813/86228910-46c11d80-bb8f-11ea-9709-410f2aec56ee.png)

Any modification you do to the F# code will be reflected in the web page after saving.

## Debugging the app

1. Set a breakpoint in VS Code (F9)
![image](https://user-images.githubusercontent.com/1781813/86229043-72dc9e80-bb8f-11ea-99e3-f88628861d04.png)
2. Run the code!
3. Use VS Code debugger to inspect call stack and variables etc.
![image](https://user-images.githubusercontent.com/1781813/86229249-bcc58480-bb8f-11ea-8aac-779b14c1c6b9.png)
![image](https://user-images.githubusercontent.com/1781813/86229276-c51dbf80-bb8f-11ea-8914-835af77e3d0c.png)
![image](https://user-images.githubusercontent.com/1781813/86229317-d070eb00-bb8f-11ea-8844-038975aa0948.png)

## Project structure

### npm

JS dependencies are declared in `package.json`, while `package-lock.json` is a lock file automatically generated.

### Webpack

[Webpack](https://webpack.js.org) is a JS bundler with extensions, like a static dev server that enables hot reloading on code changes. Fable interacts with Webpack through the `fable-loader`. Configuration for Webpack is defined in the `webpack.config.js` file. Note this sample only includes basic Webpack configuration for development mode, if you want to see a more comprehensive configuration check the [Fable webpack-config-template](https://github.com/fable-compiler/webpack-config-template/blob/master/webpack.config.js).

### F#

The sample only contains two F# files: the project (.fsproj) and a source file (.fs) in the `src` folder.

### Web assets

The `index.html` file and other assets like an icon can be found in the `public` folder.
