# JS - Snippet Good!
![](https://vsmarketplacebadge.apphb.com/version/jimmydc.js--snippet-good.svg)

## 1.6.0 Release - React Hook snippets for `useState` and `useEffect`, PropTypes bugfixes

## Features

A collection of customized snippets intended for personal use. I've gathered and modified some of them from existing packages and created the rest.

## Example (`rfpe` and `ptsr` snippets)
![rfpe snippet example](./examples/rfpe.gif)

## Supported VS Code Language Extensions

- javascript (.js)
- javascriptreact (.jsx)
- css (styled component shortcuts)

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

#### `imrus` &ndash; import React, useState

`import React, { useState } from 'react'`

---

#### `imrue` &ndash; import React, useEffect

`import React, { useEffect } from 'react'`

---

#### `imruse` or `imrues` &ndash; import React, useState and useEffect

`import React, { useState, useEffect } from 'react'`

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

#### `rfe` or `rse`(deprecated) &ndash; React functional component with export after

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

#### `rus` &ndash; React `useState` statement
*__Note__: this snippet takes the `state` placeholder and captializes the `setState` counterpart using snippet transforms. Just type whatever your `state` variable is and press "Tab" to activate the transform and move on to the next placeholder.*

*__Note of Note__: I can't get this to work with the "Vim" extension, not matter how hard I try. Sorry :(* 

```js
const [state, setState] = useState()
```

#### `rue` &ndash; React `useEffect` statement
*__Note__: I didn't place the 2nd argument of `useEffect` in this snippet, because I often do not know if I'm going to need it, or what props/state will go in there until I'm done writing it. It also becomes troublesome to delete the placeholder if you don't want it*

```js
useEffect(() => {
  
})
```


#### `rfeus` or `rfes` &ndash; React component with export after and `useState` setup
*__Note__: this snippet takes the `state` placeholder and captializes the `setState` counterpart using snippet transforms. Just type whatever your `state` variable is and press "Tab" to activate the transform and move on to the next placeholder.*

*__Note of Note__: I can't get this to work with the "Vim" extension, not matter how hard I try. Sorry :(* 

```js
import React, { useState } from 'react';

const Module = () => {
  const [state, setState] = useState()

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

#### `rfpe` &ndash; React functional component with PropTypes and export after

```js
import React from 'react';
import PropTypes from 'prop-types'

const Module = () => {
  return (
    <div>
      
    </div>
  )
}

Module.propTypes = {

}

export default Module;
```

### `pt` &ndash; PropTypes object
Useful if you have already created a component and decide you need Proptypes after. Uses the filename as the default for `Module`.
*__Note:__: VSCode snippets do not autocomplete during placeholders, so you'll want to hit escape after tabbing inside of the object*

```js
Module.propTypes = {

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

| Prefix  | Output                         |
| ------- | ------------------------------ |
| `pta`   | PropTypes.array                |
| `ptar`  | PropType.array.isRequired      |
| `ptb`   | PropType.bool                  |
| `ptbr`  | PropType.bool.isRequired       |
| `ptel`  | PropType.element               |
| `ptelr` | PropType.element.isRequired    |
| `ptf`   | PropType.func                  |
| `ptfr`  | PropType.func.isRequired       |
| `ptnd`  | PropType.node                  |
| `ptndr` | PropType.node.isRequired       |
| `ptn`   | PropType.number                |
| `ptnr`  | PropType.number.isRequired     |
| `pto`   | PropType.object                |
| `ptor`  | PropType.object.isRequired     |
| `pts`   | PropType.string                |
| `ptsr`  | PropType.string.isRequired     |
| `ptsh`   | PropType.shape({})            |
| `ptshr`  | PropType.shape({}).isRequired |

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

#### `expte` &ndash; Testing expect to equal

`expect().toEqual()`

---

#### `expte` &ndash; Testing expect to be

`expect().toBe()`

---

#### `expte` &ndash; Testing expect to be null

`expect().toBeNull()`

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

#### `rtlbs` &ndash; React Testing Library: Bootstrap

```js
import React from 'react'
import { render } from '@testing-library/react'

import TestComponent from '.'

describe('TestComponent', () => {
  test('should render', () => {
    const { container } = render(
      <TestComponent></TestComponent>
    )

    expect(container).toMatchSnapshot()
  })
})
```

---

#### `rtlss` &ndash; React Testing Library: Snapshot
`expect(container).toMatchSnapshot()`

---

#### `tst` &ndash; Testing: test block
```js
  test('', () => {
    
  })
```

---

#### `sbc` &ndash; Storybook Component
Quick story setup for a component in the same directory as the story.
```js
import React from 'react'
import { storiesOf } from '@storybook/react'

import Component from '.'

storiesOf('Components|Component', module).add('default', () => (
  <Component></Component>
))
```
---
---

## Release Notes
See [Changelog](./CHANGELOG.md)
