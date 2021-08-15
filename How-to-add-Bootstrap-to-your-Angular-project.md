# How to add Bootstrap to your Angular project

<br />

Add bootstrap 5 as an npm package like so: [https://www.npmjs.com/package/bootstrap](https://www.npmjs.com/package/bootstrap)

```
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

```
npm install @popperjs/core
```

```javascript
"scripts": [
  "./node_modules/@popperjs/core/dist/umd/popper.min.js",
  "./node_modules/bootstrap/dist/js/bootstrap.min.js"
]
```

Now lets test and see if everything works accordingly 
Add a dropdown component to your _app.component.html_

```html
<div class="dropdown">
  <button
    class="btn btn-secondary dropdown-toggle"
    type="button"
    id="dropdownMenuButton1"
    data-bs-toggle="dropdown"
    aria-expanded="false"
  >
    Dropdown button
  </button>
  <ul class="dropdown-menu" aria-labelledby="dropdownMenuButton1">
    <li><a class="dropdown-item" href="#">Action</a></li>
    <li><a class="dropdown-item" href="#">Another action</a></li>
    <li><a class="dropdown-item" href="#">Something else here</a></li>
  </ul>
</div>
```
