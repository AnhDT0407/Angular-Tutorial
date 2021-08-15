# How to add Bootstrap to your Angular project

<br />

Add bootstrap 5 as an npm package like so: [https://www.npmjs.com/package/bootstrap](https://www.npmjs.com/package/bootstrap)

```javascript
npm i bootstrap
```

In your angular.json add bootstrap stylesheet and javascript

```
"styles": [
  "src/scss/styles.scss",
  "./node_modules/bootstrap/dist/css/bootstrap.min.css",
],

"scripts": [
  "./node_modules/bootstrap/dist/js/bootstrap.min.js"
]
```

Now add popperjs and add it to your scripts

```
npm install @popperjs/core
```

```
"scripts": [
  "./node_modules/@popperjs/core/dist/umd/popper.min.js",
  "./node_modules/bootstrap/dist/js/bootstrap.min.js"
]
```
