Use the extension ID to find in VSC marketplace: Jabun.vanilla-extract-react-snippets
https://marketplace.visualstudio.com/items?itemName=Jabun.vanilla-extract-react-snippets

## Usage

After installation of this snippets, add this inside your settings

`"editor.snippetSuggestions": "top",`

## Snippets List

| Snippets | Content                              |
| -------: | ------------------------------------ |
| ivs      | import { style }                     |
| ivsv     | Import { styleVariants }             |
| ivk      | Import { keyframes }                 |
| iva      | import * as styles from './[file].css|
| vsr      | Create style rule                    |
| vesr     | Create & export style rule           |
| vsv      | Create styleVariants                 |
| vesv     | Create & export styleVariants        |
| vke      | Create keyframe                      |
| veke     | Create & export keyframe             |
| vmq      | Create media query                   |
| vse      | Create selectors                     |
| vsc      | Create style composition             |
| vesc     | Create & export  style composition   |
| vus      | Use styles in className              |
| vsp      | Use sprinkles                        |

---

### ivs [Import {style}]

```js
import { style } from '@vanilla-extract/css';
```

---

### ivsv [Import {styleVariants}]

```js
import { styleVariants } from '@vanilla-extract/css';
```

---
### ivk [Import {keyframes}]

```js
import { keyframes } from '@vanilla-extract/css';
```

---
### iva [Import * as styles from './[file].css]

```js
import * as styles from './${1:$TM_FILENAME_BASE}.css';
```

---
### vsr [Create {style} rule]

```js
const $1 = style({
    $2: $3
});
```

---
### vesr [Create & export {style} rule]

```js
export const $1 = style({
    $2: $3
});
```

---
### vsv [Create {styleVariants}]

```js
const $1 = styleVariants({
  $2: {
    $3: $4,
  },
});
```

---
### vesv [Create & export {styleVariants}]

```js
export const $1 = styleVariants({
  $2: {
    $3: $4,
  },
});
```

---
### vke [Create {keyframes}]

```js
const $1 = keyframes({
    $2: $3
});
```

---
### veke [Create & export {keyframes}]

```js
export const $1 = keyframes({
    $2: $3
});
```

---
### vmq [Create media query]

```js
'@media': {
  'screen and (min-width: $1px)': {
    $2: $3,
  },
},
```

---
### vse [Create Selectors]

```js
selectors: {
  '$1': {
    $2: $3,
  },
},
```

---
### vsc [Create Style Composition]

```js
const $1 = style([$2, { $3: $4 }]);
```

---
### vesc [Create & export Style Composition]

```js
export const $1 = style([$2, { $3: $4 }]);
```

---
### vus [Use imported styles in className]

```js
className={styles.$1}
```

---
### vsp [Use sprinkles]

```js
className={sprinkles({
  $1: $2 
})}
```
