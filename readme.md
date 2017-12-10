# Rollup Exec

> A simple way to make executable binaries for node with Rollup

## Usage

Simply include the plugin in your normal list of rollup plugins.

```js

import { rollup } from 'rollup';
import execute from 'rollup-plugin-exec';

function build() {
    return rollup({
        input: 'your/input',
        plugins: [
            // ... some plugins,
            execute()
        ]
    })
    .then(({ write }) => write({
        ....
    }))
}
```
