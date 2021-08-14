# Exports and Imports

We can import content from another file

## Example

`person.js`

```js
const person = {
    name: 'Max'
}
export default person
```

`utility.js`
```js
export const clean = () => {/*...*/}
export const baseData = 10;
```

`app.js`

```js
// default export
import person from './person.js'
import prs from './person.js'

// named export
import { baseData } from './utility.js'
import { clean } from './utility.js'
```

## Variation

```js
import person from './person.js'
import prs from './person.js'

import { smth } from './utility.js'
import { smth as Smth } from './utility.js' // can assign an allias
import * as bundled from './utility.js' // import everything with *, and assign an allias
```