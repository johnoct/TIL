<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [array-filter](#array-filter)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# array-filter

TIL that you get an array with a filter condition in javascript using the filter method.

An example:
```
const words = ['john', 'julia', 'jacob', 'smith']

const result = words.filter((word) => word.length > 4);

console.log(result);
```

Output in Node:
```
> const words = ['john', 'julia', 'jacob','smith'];
undefined
> result = words.filter((word) => word.length > 4);
[ 'julia', 'jacob', 'smith' ]
> console.log(result)
[ 'julia', 'jacob', 'smith' ]
```

Reference: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter