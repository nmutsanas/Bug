Bugs
===========

Tampermonkey wrapper around this fun script: http://auz.github.io/Bug/.

Variations
----------
To activate this script only on the 1st of April, add this after 'use strict'
```javascript
var today = new Date();
if(today.getDate() != 1 || today.getMonth() != 3){
    return;
}
```

To activate it randomly with a chance of about 5%, add this after 'use strict'
```javascript
if(Math.random() > 0.05){
        return;
    }
```
