# import-export-default

TIL that there are two different ways to export and import javascript constants and functions.

There is:
- named exports
- default exports

## Example
- isAdult is exported as a named export
- isSenior is exported as Default

eg. :
- `person.js`
```
const isAdult = (age) => age >= 18;
const canDrink = (age) => age >= 21;
const isSenior = (age) => age >= 65;

export {isAdult, canDrink, isSenior as Default};
```

- `app.js`
```
import isSenior, {isAdult, canDrink} from './person.js'
...
```

Note*: when you import the function, you can actually name it whatever if the function is exported as default.

eg.:

- `app.js`
```
import thisIsANewName, {isAdult, canDrink} from './person.js'
...
```