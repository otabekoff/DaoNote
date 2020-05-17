### Installation

```bash
npm install --save @dao-vue/note   # using npm
yarn add @dao-vue/note --save      # using npm
```

### Adding to project

```js
import Vue from 'vue'
import DaoNote from '@dao-vue/note'

Vue.use(DaoNote)
```

### Usage
```html
<dao-note color="info" message="Here is an example of Dao VueJS Note component." />
<dao-note color="success">Here is an example of Dao VueJS Note component.</dao-note>
```