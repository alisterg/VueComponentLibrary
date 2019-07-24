# Vue Component Library Starter

## Project setup
```
npm run build-bundle
```
This generates the files in dist/. 

`test.umd.js` is our UMD file, which we can use in most situations, including in a HTML script tag. Our library is also exported to a property of the **window** object in a HTML file.

`test.umd.min.js` is the minified version, which we will use in production.

`test.common.js` is our CommonJS implementation, which we can use from NodeJS with a **require** statement.

## Using in a HTML file
Include Vue.js from the CDN
```
<script src="https://cdn.jsdelivr.net/npm/vue"></script>
```
Since we already registered our components globally, we can use them in any Vue component we create.

```
<div id="app">
  <test-component>
</div>

<script>
var app = new Vue({
  el: '#app'
})
</script>
```