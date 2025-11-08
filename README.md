# is-forty-seven

[![npm version](https://img.shields.io/npm/v/is-forty-seven.svg)](https://www.npmjs.com/package/is-forty-seven)
[![npm downloads](https://img.shields.io/npm/dm/is-forty-seven.svg)](https://www.npmjs.com/package/is-forty-seven)
[![License: ISC](https://img.shields.io/badge/License-ISC-blue.svg)](https://opensource.org/licenses/ISC)

A simple, lightweight library that checks if a provided value is 47.

## Installation

```bash
npm install is-forty-seven
```

## Usage

```javascript
import isFortySeven from 'is-forty-seven';

console.log(isFortySeven(47));    // true
console.log(isFortySeven(46));    // false
console.log(isFortySeven(48));    // false
console.log(isFortySeven(0));     // false

// String examples
console.log(isFortySeven("47"));  // false (strings are not equal to numbers)
console.log(isFortySeven("forty-seven")); // false
```

## API

### `isFortySeven(value: number): boolean`

Checks if the provided value is exactly 47.

**Parameters:**
- `value` (number): The value to check (must be a number type)

**Returns:**
- `boolean`: `true` if the value is 47, `false` otherwise

**Note:** In TypeScript, passing a string (like `"47"`) will result in a compile-time error. In plain JavaScript, strings will always return `false` since strict equality (`===`) is used.

**Example:**
```javascript
import isFortySeven from 'is-forty-seven';

if (isFortySeven(47)) {
  console.log('The answer to life, the universe, and everything!');
}
```

## TypeScript Support

This library is written in TypeScript and includes type definitions. No additional `@types` package needed.

## License

ISC

## Author

Yurii Yesipov

