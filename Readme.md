> fp-ts extra string utils

```ts
import {split,join} from 'fp-ts-string'
import {pipe} from 'fp-ts/lib/pipeable'
import * as assert from 'assert'

const result = pipe(
    "a,b,c",
    split(','),
    join(':')
)

assert.deepStrictEqual(result, "a:b:c")
```
