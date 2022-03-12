# lz-ts

LZ-based compression algorithm for TypeScript projects (Browser, Node.js).
This project is a TypeScript port of the original package `lz-string` using modern tooling.

## Setup

    yarn add lz-ts

## Usage

### UTF16 encoded string compression

```ts
import { compress, decompress } from 'ls-ts'

const compressed = compress('input')
const decompressed = decompress(compressed)
```

### URI encoded string compression

```ts
import { compressToURI, decompressFromURI } from 'ls-ts'

const compressedURI = compressToURI('input')
const decompressedURI = decompressFromURI(compressed)
```

## Limitations

This project intentionally doesn't implement the `base64` encoding.

## Test

    yarn test
