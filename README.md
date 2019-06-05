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

#### `imr` &ndash; import React

`import React from 'react'`

---

#### `imrc` &ndash; import React, Component

`import React, { Component } from 'react'`

---

#### `imrpc` &ndash; import React, PureComponent

`import React, { PureComponent } from 'react'`

---

#### `impt` &ndash; import PropTypes

`import PropTypes from 'prop-types'`

---

#### `imes` &ndash; import shallow from enzyme

`import { shallow } from 'enzyme'`

---

#### `imem` &ndash; import mount from enzyme

`import { mount } from 'enzyme'`

---

#### `imesm` &ndash; import mount and shallow from enzyme

`import { shallow, mount } from 'enzyme'`

---

#### `exp` &ndash; export default module

`export default module`

---

#### `rce` &ndash; React, Component class with export after

```js
import React, { Component } from 'react';

class Module extends Component {
  render() {
    return (
      <div>
        
      </div>
    )
  }
}

export default Module;
```

---

#### `rse` or `rfe` &ndash; React functional component with export after

```js
import React from 'react';

const Module = () => {
  return (
    <div>
      
    </div>
  )
}

export default Module;
```

---

#### `rfc` &ndash; React functional component

```js
const Module = () => {
  return (
    <div>
      
    </div>
  )
}
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

#### `scp` &ndash; Styled Components: props callback

```js
${props => props.};
```

---

#### `sct` &ndash; Styled Components: theme callback

```js
${({ theme }) => theme.};
```

---

#### PropType snippets:

| Prefix  | Output                      |
| ------- | --------------------------- |
| `pta`   | PropTypes.array             |
| `ptar`  | PropType.array.isRequired   |
| `ptb`   | PropType.bool               |
| `ptbr`  | PropType.bool.isRequired    |
| `ptel`  | PropType.element            |
| `ptelr` | PropType.element.isRequired |
| `ptf`   | PropType.func               |
| `ptfr`  | PropType.func.isRequired    |
| `ptnd`  | PropType.node               |
| `ptndr` | PropType.node.isRequired    |
| `ptn`   | PropType.number             |
| `ptnr`  | PropType.number.isRequired  |
| `pto`   | PropType.object             |
| `ptor`  | PropType.object.isRequired  |
| `pts`   | PropType.string             |
| `ptsr`  | PropType.string.isRequired  |

---

#### `des` &ndash; Testing `describe` block

```js
describe('', () => {})
```

---

#### `tit` &ndash; Testing `it` block

```js
it('', () => {})
```

---

#### `expss` &ndash; Testing expect to match snapshot

`expect().toMatchSnapshot()`

---

#### `expte` &ndash; Testing expect toEqual

`expect().toEqual()`

---

#### `shal` &ndash; Enzyme shallow mount component

`const component = shallow(<Component />`

---

#### `shalp` &ndash; Enzyme shallow mount component with premade props object

`const component = shallow(<Component {...props} />`

---

#### `mnt` &ndash; Enzyme full mount component

`const component = mount(<Component />`

---

#### `mntp` &ndash; Enzyme full mount component with premade props object

`const component = mount(<Component {...props} />`

---

---

## Release Notes
See [Changelog](./CHANGELOG.md)
