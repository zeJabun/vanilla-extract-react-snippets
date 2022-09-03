## Usage

After install this snippets add this inside your settings

`"editor.snippetSuggestions": "top",`

## Snippets List

| Snippets | Content                              |
| -------: | ------------------------------------ |
| ivs      | import { style }                     |
| ivsv     | Import { styleVariants }             |
| ivk      | Import { keyframes }                 |
| iva      | import * as styles from './[file].css|
| vsr      | Create style rule                    |
| vsv      | Create styleVariants                 |
| vke      | Create keyframe                      |
| vmq      | Create media query                   |
| vse      | Create selectors                     |
| vsc      | Create style composition             |
| vus      | Use styles in className     |
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
### vsv [Create {styleVariants}]

```js
const $1 = styleVariants({
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
### vus [Use imported styles in className]

```js
className={styles.$1}
```

---
### vsp [Use sprinkles]

```js
className=sprinkle({
  $1: $2 
})
```

---