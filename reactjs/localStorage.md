<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [localStorage](#localstorage)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# localStorage

TIL that you can use local storage in the browser for js or react applications.

Example:
```
const set = localStorage.setItem('key', 'value');
const get = localStorage.getItem('key');

localStorage.setItem('name', 'John');
undefined
localStorage.getItem('name');
"John"
```

It is also not supported on node and only the Browser.

Reference: https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage