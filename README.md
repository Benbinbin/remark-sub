# remark-sub
This is a remark plugin to transform `_text_` into a `<sub>text</sub>` element.

## Install

```bash
npm install remark-sub
```

## Usage

```js
import {remark} from 'remark';
import remarkSub from 'remark-sub';

const doc = 'This is a _subscript_';
remark().use(remarkSub).process(doc).then(file => {
    console.log(String(file));
    // => This is a <sub>subscript</sub>
});
```

## License
[MIT](./LICENSE)