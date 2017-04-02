# Webpack-2
*This serves as a step-by-step, intro to the Webpack module bundler*

## 1-Geting-Started
- Objective - bundle your code and run it in th browser

## Setup
#### - *Create these files:*
- index.html
- index.js
- webpack.config.js

#### - *Run these commands:*
1. `npm init -y` - *Create a `package.json`*
2. `npm install --save-dev webpack` - *Install Webpack as a dev dependency*

#### - *Update files:*
1. `index.html`
```html
...
<body>
    <script src="bundle.js"></script>
</body>
...
```
2. `index.js`
```javascript
document.write('Hello World!!!');
```
3. `webpack.config.js`
```javascript
module.exports = {
    entry: './index.js',
    output: {
      filename: 'bundle.js'
    }
};
```
4. `package.json`
```json
...
"scripts": {
  "test": "echo \"Error: no test specified\" && exit 1",
  "build": "webpack"
},
...
```

## Running the project
1. `npm run build` - creates an output file (`bundle.js`) with our bundled code
2. Open `index.html` in the browser

## Next Steps
1. Play around, customize it to your preferences
2. Build it all again from scratch, as best as you can from memory
2. When finished `git checkout` to the next branch

