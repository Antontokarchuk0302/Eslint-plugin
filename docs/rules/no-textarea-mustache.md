# Disallow mustaches in `<textarea>` (no-textarea-mustache)

> Interpolation on textareas (`<textarea>{{text}}</textarea>`) won't work. Use `v-model` instead.
>
> https://vuejs.org/v2/guide/forms.html#Multiline-text

## 📖 Rule Details

This rule reports mustaches in `<textarea>`.

👎 Examples of **incorrect** code for this rule:

```html
<template>
    <textarea>{{message}}</textarea>
</template>
```

👍 Examples of **correct** code for this rule:

```html
<template>
    <textarea v-model="message"></textarea>
</template>
```

## 🔧 Options

Nothing.
