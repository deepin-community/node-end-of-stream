# Installation
> `npm install --save @types/end-of-stream`

# Summary
This package contains type definitions for end-of-stream (https://github.com/mafintosh/end-of-stream).

# Details
Files were exported from https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/end-of-stream.
## [index.d.ts](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/end-of-stream/index.d.ts)
````ts
// Type definitions for end-of-stream 1.4
// Project: https://github.com/mafintosh/end-of-stream
// Definitions by: Sami Kukkonen <https://github.com/strax>
// Definitions: https://github.com/DefinitelyTyped/DefinitelyTyped
/// <reference types="node"/>

interface Options {
  readable?: boolean | undefined;
  writable?: boolean | undefined;
  error?: boolean | undefined;
}
type Stream = NodeJS.ReadableStream | NodeJS.WritableStream;
type Callback = (error?: Error | null) => void;
declare function eos(
  stream: Stream,
  callback?: Callback
): () => void;
declare function eos(
  stream: Stream,
  options: Options,
  callback?: Callback
): () => void;
declare namespace eos {
}
export = eos;

````

### Additional Details
 * Last updated: Tue, 06 Jul 2021 19:03:13 GMT
 * Dependencies: [@types/node](https://npmjs.com/package/@types/node)
 * Global values: none

# Credits
These definitions were written by [Sami Kukkonen](https://github.com/strax).
