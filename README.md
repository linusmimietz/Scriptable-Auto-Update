# Scriptable Auto Update
This simple wrapper for your [Scriptable](https://scriptable.app) code automatically updates it locally every day.
  
![Loop GIF](https://i.imgur.com/iEFhyVq.gif)

## Features
* Automatically downloades your latest code every day from a URL
* If the update fails, it uses the latest locally available version
* Cleans up old locally saved versions automatically
* Executes your code every time it gets run

## Usage
The wrapper will run the main() function of your code everytime it get's executed. Therefore it's necessary to export the function at the end of your code like so:
```javascript
module.exports = {
  main
};
```
Copy the content from main.js and replace the scriptName and scriptUrl with your parameters. Then simply paste it into Scriptable!

## Example
Take a look inside the example folder to see an implementation.  
Wanna try it out? Then simply copy the content of example/main.js and paste it into Scriptable!

## License
This repository is available under the [MIT license](https://opensource.org/licenses/MIT).
