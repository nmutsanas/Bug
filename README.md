Bugs
===========

Tampermonkey wrapper around this fun script: http://auz.github.io/Bug/.

Instructions
------------
How to [install tampermonkey scripts](http://tampermonkey.net/faq.php#Q102). 
- Remember to adjust the ```@match``` parameter to target the pages you want to bug.
- Adjust the ```BugController``` and ```SpiderController``` as [documented](http://auz.github.io/Bug/) to your liking.

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
