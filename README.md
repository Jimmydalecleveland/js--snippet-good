# JS - Snippet Good!

## Features

A collection of customized snippets intended for personal use. I've gathered and modified some of them from existing packages and created the rest.

## Supported VS Code Language Extensions

- javascript (.js)
- javascriptreact (.jsx)

## Snippets

#### `cl` &ndash; console log
`console.log()`

---

#### `clc` &ndash; console log
_note:_ cursor starts at your message, first tab goes to color, third tab goes to the position after the css string, so you can add additional variables to log.

`console.log('%cYourTextHere', 'color: cornflowerblue;')`

---

#### `imp` &ndash; import module
`import module from 'module'`

---

#### `imd` &ndash; import module destructured
`import { moduleName } from 'module'`

---

#### `imrpc` &ndash; import React, PureComponent
`import React, { PureComponent } from 'react'`

---

#### `exp` &ndash; export default module
`export default module` 

---
#### `rce` &ndash; React, Component class with export after 
```js
import React, { Component } from 'react'

class Module extends Component {
  render() {
    return (
      <div>

      </div>
    )
  }
}

export default Module 
```
---

#### `rse` &ndash; React stateless functional component
```js
import React from 'react'

const Module = () => {
  return (
    <div>

    </div>
  )
}

export default Module 
```
---
---

## Release Notes

### 0.0.1

Initial release. Just a few snippets to start with.
