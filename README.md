# @ctx-core/svelte-preprocess

Preprocessing scripts for svelte

## Install

```shell
npm i @ctx-core/svelte-preprocess
```

## Preprocess

```javascript
// rollup.config.js
import { proprocess_ } from '@ctx-core/svelte/node'
const preprocess = proprocess_([
	// preprocess object 1,
	// preprocess object 2,
])
export default {
	client: {
		//...
		plugins: [
			// ...
			svelte({
				// ...
				preprocess,
			}),
			// ...
		],
		// ...
	},
	server: {
		//...
		plugins: [
			// ...
			svelte({
				// ...
				preprocess,
			}),
			// ...
		],
		// ...
	},
	serviceworker: {
		// ...
	},
}
```
