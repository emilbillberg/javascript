# JavaScript Style Guide
The style guide is heavily influenced from [Airbnb's Javascript Style Guide](https://github.com/airbnb/javascript)

## Objects
1. Use the literal syntax for object creation.
```
const bad = new Object();

const good = {};
```

2. Use property value shorthand.
```
const description = 'My desctiption';

const bad = {
  description: description,
};

const good = {
  description,
};
```

3. Use object method shorthand.
```
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
```
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
```
const bad = new Array();

const good = [];
```

2. Use array spreads `...` to copy arrays.
```
const good = [...array];
```

## Strings
1. Use single quotes '' for strings.
```
const good1 = 'Hello, world!';
```

2. When programmatically building up strings, use template strings instead of concatenation.
```
const name = 'Batman';

const bad = 'Hello ' + name + '! How are you?';

const good = `Hello ${name}! How are you?`;
```




