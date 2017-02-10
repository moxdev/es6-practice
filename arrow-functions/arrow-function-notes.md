# Arrow Functions

- Arrow Functions are anonymous functions
- can be saved in a variable

```javascript

const bands = ['Tool', 'Iron Maiden', 'Black Sabbath'];

// old anonymous function
const favoriteBands = bands.map(function (name) {
    return `${name} rocks`;
});

// new arrow function
const favoriteBands2 = bands.map((name) => {
   return `${name} rocks`;
});

// arrow function same way without parenthesis (stylistic choice)
const favoriteBands3 = bands.map(name => {
   return `${name} rocks`;
});

// arrow function has implicit return so no need for return statement or curly brackets
const favoriteBands4 = bands.map( (name) => `${name} rocks` );

// arrow function with no parameters requires empty parens ()
const favoriteBands5 = bands.map( () => `Metal rocks` );

// saved in a variable, behaves more like a named function but is still anonymous
const metalBand = (band) => { console.log(`My favorite Metal band is ${band}!`) }

console.log(favoriteBands);
console.log(favoriteBands2);
console.log(favoriteBands3);
console.log(favoriteBands4);
console.log(favoriteBands5);
metalBand('Opeth');
```