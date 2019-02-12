# Objects

Objects are collections of related properties (key/value pairs).

## Creating objects

```js
const dog = { name: 'spot' }
console.log(dog);
```

```js
const cat = {
  name: 'fluffy'
};
console.log(cat);
```

```js
const rover = {
  name: 'rover',
  age: 15
};
console.log(rover);
```

Objects are created by adding properties between curly braces separated by commas.
Each property is comprised of a key and a value separated by a colon. The key is a
string and the value can be anything.

## Accessing properties

### Dot Notation

```js
const dog = {
  name: 'spot',
  age: 1
};
console.log(dog.name);
```

```js
const dog = {
  name: 'spot',
  age: 1
};
console.log(dog.age);
```

Dot notation access object properties by providing the property key
after a dot (e.g. `object.key`).

### Bracket Notation

```js
const dog = {
  name: 'spot',
  age: 1
};
console.log(dog['name']);
```

```js
const dog = {
  name: 'spot',
  age: 1
};
console.log(dog['age']);
```

Bracket notation accesses the object properties by providing the property
key inside square brackets (e.g. `object['key']`).

## Setting properties

### Dot Notation

```js
const dog = {
  name: 'spot',
  age: 1
};
dog.name = 'rover'
console.log(dog)
```

```js
const dog = {
  name: 'spot',
  age: 1
};
dog.age = 15;
console.log(dog)
```

### Bracket Notation

```js
const dog = {
  name: 'spot',
  age: 1
};
dog['name'] = 'bingo';
console.log(dog)
```

### Adding new properties

```js
const dog = {
  name: 'spot',
  age: 1
};
dog.legs = 4;
console.log(dog)
```

```js
const dog = {
  name: 'spot',
  age: 1
};
dog['weight'] = '5 lbs';
console.log(dog)
```

New properties can also be added with either dot or bracket notation

## Deleting properties

```js
const dog = {
  name: 'spot',
  age: 1,
  legs: 4,
  weight: '5 lbs'
};
delete dog.name;
console.log(dog);
```

```js
const dog = {
  name: 'spot',
  age: 1,
  legs: 4,
  weight: '5 lbs'
};
delete dog['name'];
console.log(dog);
```

```js
const dog = {
  name: 'spot',
  age: 1,
  legs: 4,
  weight: '5 lbs'
};
delete dog['name'];
delete dog.age;
console.log(dog);
```

## Dynamic properties

```js
const dog = {
  name: 'spot',
  age: 1
};
const key = 'name';
console.log(dog.key);
console.log(dog[key])
```

When we are dealing with dynamic property access (accessing properties by a key
bound to a name (i.e. `const key = 'name')`) we must use bracket notation.

```js
const dog = {
  name: 'spot',
  age: 1
};
const key = 'name';
console.log(dog['name'] === dog[key]);
console.log('name' === key)
```

```js
const dog = {
  name: 'spot',
  age: 1,
  legs: 4,
  weight: '40 lbs'
};

const keys = ['name', 'age', 'legs', 'weight'];
for(let i = 0; i < keys.length; i++) {
  const key = keys[i];
  console.log(dog[key]);
}
```
