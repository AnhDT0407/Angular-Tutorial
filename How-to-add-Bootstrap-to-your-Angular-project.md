# How to add Bootstrap to your Angular project

<br />

Add bootstrap 5 as an npm package like so: [https://www.npmjs.com/package/bootstrap](https://www.npmjs.com/package/bootstrap)

```npm
npm i bootstrap
```

In your angular.json add bootstrap stylesheet and javascript

```javascript
"styles": [
  "src/scss/styles.scss",
  "./node_modules/bootstrap/dist/css/bootstrap.min.css",
],

"scripts": [
  "./node_modules/bootstrap/dist/js/bootstrap.min.js"
]
```

Now add popperjs and add it to your scripts

```javascript
npm install @popperjs/core
```

```javascript
"scripts": [
  "./node_modules/@popperjs/core/dist/umd/popper.min.js",
  "./node_modules/bootstrap/dist/js/bootstrap.min.js"
]
```
