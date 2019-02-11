# Objects

## Creating objects

```js
const dog = { name: 'spot' }
dog
```

```js
const cat = {
  name: 'fluffy'
};
cat
```

```js
const rover = {
  name: 'rover',
  age: 15
};
rover
```

## Accessing properties

```js
const dog = {
  name: 'spot',
  age: 1
};
dog.name
```

```js
dog.age
```

```js
dog['name']
```

```js
dog['age']
```

```js
const key = 'name';
dog.key;
dog[key];
```

## Setting properties

```js
const dog = {
  name: 'spot',
  age: 1
};
dog.name = 'rover'
dog
```

```js
dog.age = 15;
dog
```

```js
dog['name'] = 'bingo';
dog
```

```js
dog.legs = 4;
dog
```

```js
dog['weight'] = '5 lbs';
dog
```
