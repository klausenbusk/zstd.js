*This is mostly a POC and isn't used in production, you have been warned!*

[`zstd`](https://github.com/facebook/zstd/) in the browser, because why not? ;)

## Build
```
$ git clone --recurse-submodules https://github.com/klausenbusk/zstd.js.git
$ cd zstd.js
$ make
```

## Usage
```javascript
const zstd = await ZSTD();

zstd.compress(<Uint8Array>, <compressionLevel>) <Uint8Array>
zstd.decompress(<Uint8Array>) <Uint8Array>
zstd.compressString(<string>) <Uint8Array>
zstd.decompressString(<Uint8Array>) <string>
```
See also: [example.html](./example.html)
