# \<udes-moment\>
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/UdeSElements/udes-moment)

`udes-moment` is a Polymer 2 wrapper for the [Moment.js](https://momentjs.com/)
library. 

There are currently **2** components and **1** mixin available:
- Components
  - \<udes-moment\>
  - \<udes-moment-interval\>
- Mixin
  - UdeS.MomentMixin
  
The `UdeS.MomentImportMixin` is not intented to be use outside this repositery.

All the components and mixins use the `UdeS.LanguageMixin` to automatically 
update the date according to the global language.

## What should I use?
You should use the `UdeS.MomentMixin` if you have many dates to format inside
you component. If you have only one or two, use the components instead.

## Configuration
If you use one of the components or one of the mixins, you need to update your 
`polymer.json` to includes the Moment.js files:
```json
{
  "extraDependencies": [
    "bower_components/moment/min/moment.min.js",
    "bower_components/moment/locale/*.js"
  ],
}
```

You also need to update your `sw-precache-config.js` accordingly:
```javascript
/* eslint-disable-next-line no-undef */
module.exports = {
  staticFileGlobs: [
    'bower_components/moment/locale/*',
    'bower_components/moment/min/moment.min.js',
  ],
};
```

## Demo
<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="demo/udes-moment-demo.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<udes-moment-demo></udes-moment>
```
