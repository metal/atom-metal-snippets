# Atom Metal.js Snippets
[![apm](https://img.shields.io/apm/v/atom-metal-snippets.svg?style=flat-square)](https://atom.io/packages/atom-metal-snippets)
[![apm](https://img.shields.io/apm/dm/atom-metal-snippets.svg?style=flat-square)](https://atom.io/packages/atom-metal-snippets)

An [Atom](https://atom.io/) snippet library for [Metal.js](https://github.com/metal/metal), and [metal-css-transitions](https://github.com/metal/metal-css-transitions). This library uses ES6 syntax.

Install via `apm install atom-metal-snippets`

## Includes

Imports
---

#### [ict]
```js
import Transition from 'metal-css-transitions';
```

#### [ijsx]
```js
import Component from 'metal-jsx';
```

#### [imr]
```js
import ${1} from 'metal-redux';
```

#### [isoy]
```js
import Component from 'metal-soy';
```

Soy
---

#### [soy]
```js
import Component, {Config} from 'metal-soy';

import templates from './${1:MyComponent}.soy';

class ${1:MyComponent} extends Component {
	${2:}
}

${1:MyComponent}.STATE = {
};

Soy.register(${1:MyComponent}, templates);

export default ${1:MyComponent};
```

JSX
---

#### [bind]
```js
this.${1} = this.${1}.bind(this);
```

#### [jsx]
```js
import Component, {Config} from 'metal-jsx';

class ${1:MyComponent} extends Component {
	render() {
		return (
			${2:<div>MyComponent</div>}
		);
	}
}

${1:MyComponent}.PROPS = {
};

${1:MyComponent}.STATE = {
};

export default ${1:MyComponent};
```

#### [trans]
```js
<Transition name="$1">
		${2}
</Transition>
```

Life Cycles
---

#### [att]
```js
attached() {
	${1}
}
```

#### [cre]
```js
created() {
	${1}
}
```

#### [det]
```js
detached() {
	${1}
}
```

#### [dis]
```js
disposed() {
	${1}
}
```

#### [ren]
```js
render() {
	return (
		${2}
	);
}
```

#### [rend]
```js
rendered() {
	${1}
}
```

#### [shup]
```js
shouldUpdate(newState, newProps) {
	${1}
}
```

#### [sync]
```js
sync$1(newVal, prevVal) {
	${2}
}
```

State Management
---

#### [sst]
```js
this.setState({$1});
```

#### [PRO]
```js
${1}.PROPS = {
	${2}
};
```

#### [STA]
```js
${1}.STATE = {
	${2}
};
```

Types
---

#### [conan]
```js
Config.any()
```

#### [conarr]
```js
Config.array()
```

#### [conarro]
```js
Config.arrayOf(${1})
```

#### [conboo]
```js
Config.bool()
```

#### [confun]
```js
Config.func()
```

#### [conino]
```js
Config.instanceOf(${1})
```

#### [connum]
```js
Config.number()
```

#### [conob]
```js
Config.object()
```

#### [conobo]
```js
Config.objectOf(${1})
```

#### [conoot]
```js
Config.oneOfType(
	[
		${1},
	]
)
```

#### [consha]
```js
Config.shapeOf(
	{
		${1}
	}
)
```

#### [constr]
```js
Config.string()
```

#### [conval]
```js
Config.value(${1})
```
