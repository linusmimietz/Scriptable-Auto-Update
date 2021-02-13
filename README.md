# Scriptable Auto Update
This simple wrapper for your [Scriptable](https://scriptable.app) code automatically updates it locally every day.
  
![Loop GIF](https://i.imgur.com/iEFhyVq.gif)

## Why did I develop it?
I'm a big fan of the [Scriptable](https://scriptable.app) app. It's an excellent tool for creating custom widgets, for example. When sharing your code with other people, I didn't find an easy way to fix bugs or add features afterward. This wrapper aims to solve this challenge.

## Features
* Automatically downloads your latest code every day from a URL
* If the update fails, it uses the latest locally available version
* Cleans up old locally saved versions automatically
* Executes your code every time it gets run

## Usage
The wrapper will run the main() function of your code every time it gets executed. Therefore it's necessary to export the function at the end of your file like so:
```javascript
module.exports = {
  main
};
```
Copy the content from *main.js* and replace the `scriptName` and `scriptUrl` with your custom values. Then simply paste it into Scriptable. The wrapper will automatically load and update your code from the URL.

## Example
Take a look inside the example folder to see an implementation.  
Want to try it out? Then simply copy the content of *example/main.js* and paste it into Scriptable!

## License
This repository is available under the [MIT license](https://opensource.org/licenses/MIT).
