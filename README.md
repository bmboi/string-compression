# JS Compression Library

The JS Compression Library is a lightweight JavaScript library that implements a simple character mapping technique to reduce the size of strings. It can be used to compress and decompress strings, achieving up to 80% reduction in size.

## Background

When transmitting or storing large amounts of textual data, it is often desirable to reduce the size of the data to optimize network bandwidth or storage space. The JS Compression Library utilizes a character mapping technique inspired by reverse Base64 encoding to achieve compression.

## Installation

To use the JS Compression Library, you can either include the library file in your HTML file or require it in your Node.js application.

### Browser

```html
<script src="compression-library.js"></script>
```

### Node.js

Install the library using npm:

```shell
npm install compression-library
```

Then require it in your Node.js application:

```javascript
const CompressionLibrary = require('compression-library');
```

## Usage

The JS Compression Library provides two methods: `compress` and `decompress`. Here's how to use them:

```javascript
// Compressing a string
const originalString = 'Hello, World!';
const compressedString = CompressionLibrary.compress(originalString);
console.log('Compressed string:', compressedString);

// Decompressing a string
const decompressedString = CompressionLibrary.decompress(compressedString);
console.log('Decompressed string:', decompressedString);
```

The `compress` method takes a string as input and returns the compressed version of the string. The `decompress` method takes a compressed string as input and returns the original decompressed string.

## Limitations

- The character mapping technique used in the library is simple and may not handle all possible characters or encoding scenarios. It is recommended for basic text compression needs.
- The library is not designed for encrypting or securing data. It focuses solely on reducing the size of strings.

## License

This library is released under the [MIT License](https://opensource.org/licenses/MIT).
