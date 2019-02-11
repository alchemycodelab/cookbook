# Function syntax

```js
function printHello() {
  console.log('hello');
}

printHello();
```

```js
printHello();
```

```js
function print(text) {
  console.log(text);
}

print('hi there');
```

```js
print('Welcome!');
```

```js
function printWithTitle(title, text) {
  console.log(title);
  console.log(text);
}

printWithTitle('A function', 'hi there');
```

```js
printWithTitle('hello', 'Welcome');
```

```js
function concat(firstPart, secondPart) {
  const together = firstPart + secondPart;
  return together;
}

concat('hi ', 'there');
```

```js
function concat(firstPart, secondPart) {
  return firstPart + secondPart;
}

concat('hi ', 'there');
```

```js
function add(a, b) {
  return a + b;
}

add(1, 3);
add(4, 5);
```

```js
function sum(numbers) {
  let sum = 0;
  for(let index = 0; index < numbers.length; i++) {
    sum += numbers[index];
  }

  return sum;
}
sum([1, 2, 3]);
```
