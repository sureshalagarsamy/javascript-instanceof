# JavaScript "instanceof"

The ```instanceof``` operator allows to check whether an object belongs to a certain class. It also takes inheritance into account.

### The instanceof operator

The syntax is:

> obj instanceof Class

It returns true if obj belongs to the Class (or a class inheriting from it).

For example:

```javascript
class Rabbit {}
var rabbit = new Rabbit();

// is it an object of Rabbit class?
alert( rabbit instanceof Rabbit );	// true
```

It also works with constructor functions:

```javascript
function ABC() {}

alert( new ABC() instanceof ABC ); // true
```

…And with built-in classes like Array:

```javascript
var myArray = [1, 2, 3];
alert( myArray instanceof Array ); // true
alert( myArray instanceof Object ); // true
```
