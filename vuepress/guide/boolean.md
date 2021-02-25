# Boolean localization

:::tip Support Version
:new: 8.0+
:::

You can localize booleans with your definition formats.

*Your template will need to use `$tb()` instead of `$t()`.*

Boolean formats below:

```js
const messages = {
  en: {
    agree: 'yes | no',
    button: 'on | off',
    answer: 'correct | incorrect'
  }
}
```

Template below:

```html
<p>{{ $tb('agree', true) }}</p>
<p>{{ $tb('button', false) }}</p>
<p>{{ $tb('answer', true) }}</p>
```

Output below:

```html
<p>yes</p>
<p>off</p>
<p>correct</p>
```
