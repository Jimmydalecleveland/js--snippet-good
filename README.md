# JS - Snippet Good!

![](https://vsmarketplacebadge.apphb.com/version/jimmydc.js--snippet-good.svg)

## Newest Release: v1.7.0 - Typescript Support!
---

# Features

A collection of customized snippets intended for personal use. I've gathered and modified some of them from existing packages and created the rest.

## Example (`rfpe` and `ptsr` snippets)

![rfpe snippet example](./examples/rfpe.gif)

## Supported VS Code Language Extensions

- javascript (.js)
- javascriptreact (.jsx)
- typescript (.ts)
- typescriptreact (.tsx)
- css (styled component shortcuts)

## Debugging developer note:

If you are working on this extension, you can use the `F5` key to enter debugging mode and use the snippets you are adding/modifying in any project you like.

## Snippets

#### `cl` &ndash; `c`onsole `l`og

`console.log()`

---

#### `clc` &ndash; `c`onsole `l`og with `c`olor

_note:_ cursor starts at your message, first tab goes to color, third tab goes to the position after the css string, so you can add additional variables to log.

`console.log('%cYourTextHere', 'color: cornflowerblue;')`

---

#### `clg` &ndash; `c`onsole `l`og `g`roup

_note:_ the string passed to `.group` and `.groupEnd` should be the same

```js
console.group("Group Name");
console.log("I am in the group!");
console.groupEnd("Group Name");
```

---

#### `imp` &ndash; `imp`ort module

`import module from 'module'`

---

#### `imd` &ndash; `im`port module `d`estructured

`import { moduleName } from 'module'`

---

#### `imr` &ndash; `im`port `r`eact

`import React from 'react'`

---

#### `imrc` &ndash; `im`port `r`eact and `C`omponent

`import React, { Component } from 'react'`

---

#### `imrpc` &ndash; `im`port `r`eact and `P`ure`C`omponent

`import React, { PureComponent } from 'react'`

---

#### `imrus` &ndash; `im`port `r`eact and `u`se`S`tate

`import React, { useState } from 'react'`

---

#### `imrue` &ndash; `im`port `r`eact and `u`se`E`ffect

`import React, { useEffect } from 'react'`

---

#### `imruse` or `imrues` &ndash; `im`port `r`eact, `u`se`S`tate and use`E`ffect

`import React, { useState, useEffect } from 'react'`

---

#### `impt` &ndash; `im`port `P`rop`T`ypes

`import PropTypes from 'prop-types'`

---

#### `imes` &ndash; `im`port `e`nzyme's `s`hallow module

`import { shallow } from 'enzyme'`

---

#### `imem` &ndash; `im`port `e`nzyme's `m`ount module

`import { mount } from 'enzyme'`

---

#### `imesm` &ndash; `im`port `e`nzyme's `s`hallow and `m`ount modules

`import { shallow, mount } from 'enzyme'`

---

#### `exp` &ndash; `exp`ort default module

`export default module`

---

#### `rce` &ndash; `R`eact `C`omponent class with `e`xport after

```js
import React, { Component } from "react";

class Module extends Component {
  render() {
    return <div></div>;
  }
}

export default Module;
```

---

#### `rfe` or `rse`(deprecated) &ndash; `R`eact `f`unctional component with `e`xport after

```js
import React from "react";

const Module = () => {
  return <div></div>;
};

export default Module;
```

---

#### `rus` &ndash; `R`eact `u`se`S`tate statement

_**Note**: this snippet takes the `state` placeholder and captializes the `setState` counterpart using snippet transforms. Just type whatever your `state` variable is and press "Tab" to activate the transform and move on to the next placeholder._

_**Note of Note**: I can't get this to work with the "Vim" extension, not matter how hard I try. Sorry :(_

```js
const [state, setState] = useState();
```

#### `rue` &ndash; `R`eact `u`se`E`ffect statement

_**Note**: I didn't place the 2nd argument of `useEffect` in this snippet, because I often do not know if I'm going to need it, or what props/state will go in there until I'm done writing it. It also becomes troublesome to delete the placeholder if you don't want it_

```js
useEffect(() => {});
```

#### `rfeus` or `rfes` &ndash; `R`eact `f`unctional component with `e`xport after and `u`se`S`tate setup

_**Note**: this snippet takes the `state` placeholder and captializes the `setState` counterpart using snippet transforms. Just type whatever your `state` variable is and press "Tab" to activate the transform and move on to the next placeholder._

_**Note of Note**: I can't get this to work with the "Vim" extension, not matter how hard I try. Sorry :(_

```js
import React, { useState } from "react";

const Module = () => {
  const [state, setState] = useState();

  return <div></div>;
};

export default Module;
```

---

#### `rfc` &ndash; `R`eact `f`unctional `c`omponent

```js
const Module = () => {
  return <div></div>;
};
```

---

#### `rfpe` &ndash; `R`eact `f`unctional component with `P`ropTypes and `e`xport after

```js
import React from "react";
import PropTypes from "prop-types";

const Module = () => {
  return <div></div>;
};

Module.propTypes = {};

export default Module;
```

#### `pt` &ndash; `P`rop`T`ypes object

Useful if you have already created a component and decide you need Proptypes after. Uses the filename as the default for `Module`.
_**Note:**: VSCode snippets do not autocomplete during placeholders, so you'll want to hit escape after tabbing inside of the object_

```js
Module.propTypes = {};
```

---

#### `cdu` &ndash; React: `c`omponent`D`id`U`pdate

```js
componentDidUpdate(prevProps, prevState) {

}
```

---

#### `cdm` &ndash; React: `c`omponent`D`id`M`ount

```js
componentDidMount() {

}
```

---

#### `cdml` &ndash; React: `c`omponent`D`id`M`ount with `l`og

```js
componentDidMount() {
  console.log('Module Mounted')
}
```

---

#### `cdmlc` &ndash; React: `c`omponent`D`id`M`ount with `l`og (`c`olor)

```js
componentDidMount() {
  console.log('%cModule Mounted', 'color: cornflowerblue;')
}
```

---

#### `scp` &ndash; `S`tyled `C`omponents: `p`rops callback

```js
${props => props.};
```

---

#### `sct` &ndash; `S`tyled `C`omponents: `t`heme callback

```js
${({ theme }) => theme.};
```

---

#### PropType snippets:

| Prefix  | Output                        |
| ------- | ----------------------------- |
| `pta`   | PropTypes.array               |
| `ptar`  | PropType.array.isRequired     |
| `ptb`   | PropType.bool                 |
| `ptbr`  | PropType.bool.isRequired      |
| `ptel`  | PropType.element              |
| `ptelr` | PropType.element.isRequired   |
| `ptf`   | PropType.func                 |
| `ptfr`  | PropType.func.isRequired      |
| `ptnd`  | PropType.node                 |
| `ptndr` | PropType.node.isRequired      |
| `ptn`   | PropType.number               |
| `ptnr`  | PropType.number.isRequired    |
| `pto`   | PropType.object               |
| `ptor`  | PropType.object.isRequired    |
| `pts`   | PropType.string               |
| `ptsr`  | PropType.string.isRequired    |
| `ptsh`  | PropType.shape({})            |
| `ptshr` | PropType.shape({}).isRequired |

---

#### `des` &ndash; Testing `des`cribe block

```js
describe("", () => {});
```

---

#### `tit` &ndash; `T`esting `it` block

```js
it("", () => {});
```

---

#### `expss` &ndash; Testing `exp`ect to match `s`nap`s`hot

`expect().toMatchSnapshot()`

---

#### `expte` or `exp==` &ndash; Testing `exp`ect `t`o `e`qual

`expect().toEqual()`

---

#### `exptb` &ndash; Testing `exp`ect `t`o `b`e

`expect().toBe()`

---

#### `exptbn` &ndash; Testing `exp`ect `to `b`e `n`ull

`expect().toBeNull()`

---

#### `shal` &ndash; Enzyme `shal`low mount component

`const component = shallow(<Component />`

---

#### `shalp` &ndash; Enzyme `shal`low mount component with premade `p`rops object

`const component = shallow(<Component {...props} />`

---

#### `mnt` &ndash; Enzyme full `m`ou`nt` component

`const component = mount(<Component />`

---

#### `mntp` &ndash; Enzyme full `m`ou`nt` component with premade `p`rops object

`const component = mount(<Component {...props} />`

---

#### `rtlbs` &ndash; `R`eact `T`esting `L`ibrary: `B`oot`s`trap

```js
import React from "react";
import { render } from "@testing-library/react";

import TestComponent from ".";

describe("TestComponent", () => {
  test("should render", () => {
    const { container } = render(<TestComponent></TestComponent>);

    expect(container).toMatchSnapshot();
  });
});
```

---

#### `rtlss` &ndash; `R`eact `T`esting `L`ibrary: `S`nap`s`hot

`expect(container).toMatchSnapshot()`

---

#### `tst` &ndash; Testing: `t`e`st` block

```js
test("", () => {});
```

---

#### `sbc` &ndash; `S`tory`b`ook `C`omponent

Quick story setup for a component in the same directory as the story.

```js
import React from "react";
import { storiesOf } from "@storybook/react";

import Component from ".";

storiesOf("Components|Component", module).add("default", () => (
  <Component></Component>
));
```

---

## Typescript Snippets

#### `sbc` &ndash; `s`tory`b`ook `c`omponent

Quick story setup for a component in the same directory as the story.

```tsx
import { ComponentStory, ComponentMeta } from '@storybook/react'

import { Example } from './'

export default {
  title: 'Components/Example',
  component: Example,
} as ComponentMeta<typeof Example>

const Template: ComponentStory<typeof Example> = (args) => <Example {...args} />

export const Default = Template.bind({})
Default.args = {
  children: 'I am the Example Component',
}
```

---

## Release Notes

See [Changelog](./CHANGELOG.md)
