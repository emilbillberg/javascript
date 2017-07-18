# JavaScript Style Guide
The style guide is heavily influenced from [Airbnb's Javascript Style Guide](https://github.com/airbnb/javascript)

## Objects
1. Use the literal syntax for object creation.
```javascript
const bad = new Object();

const good = {};
```

2. Use property value shorthand.
```javascript
const description = 'My desctiption';

const bad = {
  description: description,
};

const good = {
  description,
};
```

3. Use object method shorthand.
```javascript
const bad = {
  hello: function(name) {
    console.log(`Hello, ${name}!`);
  }
};

const good = {
  hello(name) {
    console.log(`Hello, ${name}!`);
  }
};
```

4. Only quote properties that are invalid identifiers.
```javascript
const bad = {
  'one': 1,
  'two': 2,
};

const good = {
  one: 1,
  two: 2,
};
```

## Arrays
1. Use the literal syntax for array creation.
```javascript
const bad = new Array();

const good = [];
```

2. Use array spreads `...` to copy arrays.
```javascript
const good = [...array];
```

## Strings
1. Use single quotes '' for strings.
```javascript
const good1 = 'Hello, world!';
```

2. When programmatically building up strings, use template strings instead of concatenation.
```javascript
const name = 'Batman';

const bad = 'Hello ' + name + '! How are you?';

const good = `Hello ${name}! How are you?`;
```




