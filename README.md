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

#### `clc` &ndash; console log with color
_note:_ cursor starts at your message, first tab goes to color, third tab goes to the position after the css string, so you can add additional variables to log.

`console.log('%cYourTextHere', 'color: cornflowerblue;')`

---

#### `clg` &ndash; console log group
_note:_ the string passed to `.group` and `.groupEnd` should be the same

```js
  console.group('Group Name')
    console.log('I am in the group!')
  console.groupEnd('Group Name')
```

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

#### `cdu` &ndash; React: componentDidUpdate
```js
componentDidUpdate(prevProps, prevState) {

}
```

---

#### `cdm` &ndash; React: componentDidMount
```js
componentDidMount() {

}
```

---

#### `cdml` &ndash; React: componentDidMount with log
```js
componentDidMount() {
  console.log('Module Mounted')
}
```

---

#### `cdmlc` &ndash; React: componentDidMount with log (color)
```js
componentDidMount() {
  console.log('%cModule Mounted', 'color: cornflowerblue;')
}
```

---

#### PropType snippets:
| Prefix | Output |
| ------ | ------ |
| `pta`  | PropTypes.array |
| `ptar` | PropType.array.isRequired |
| `ptb`  | PropType.bool |
| `ptbr`  | PropType.bool.isRequired |
| `ptel`  | PropType.element |
| `ptelr`  | PropType.element.isRequired |
| `ptf`  | PropType.func |
| `ptfr`  | PropType.func.isRequired |
| `ptnd`  | PropType.node |
| `ptndr`  | PropType.node.isRequired |
| `ptn`  | PropType.number |
| `ptnr`  | PropType.number.isRequired |
| `pto`  | PropType.object |
| `ptor`  | PropType.object.isRequired |
| `pts`  | PropType.string |
| `ptsr`  | PropType.string.isRequired |
---

## Release Notes

### 0.0.1

Initial release. Just a few snippets to start with.

### 0.1.0

Add console log snippets

### 0.2.0

Add console.group, React lifecycle methods, and PropTypes