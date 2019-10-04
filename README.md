This repo shows how to use package.json to load different versions of Elix, and how to load different versions of Elix on the same page.

The `package.json` file creates aliases for multiple versions of Elix:

```json
"dependencies": {
  "elix-7": "npm:elix@7.0.0",
  "elix-8": "npm:elix@8.0.0"
}
```

These aliases are then referenced in paths in index.html, in HTML:

```html
<script type="module" src="node_modules/elix-7/src/DateComboBox.js"></script>
```

or in JavaScript:

```js
import DateComboBox from './node_modules/elix-8/src/DateComboBox.js';
```