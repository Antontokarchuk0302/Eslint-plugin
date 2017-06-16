# Require `v-bind:is` of `<component>` elements (require-component-is)

> You can use the same mount point and dynamically switch between multiple components using the reserved `<component>` element and dynamically bind to its `is` attribute:
>
> https://vuejs.org/v2/guide/components.html#Dynamic-Components

## 📖 Rule Details

This rule reports the `<component>` elements which do not have `v-bind:is` attributes.

👎 Examples of **incorrect** code for this rule:

```html
<template>
    <component></component>
</template>
```

👍 Examples of **correct** code for this rule:

```html
<template>
    <component :is="type"></component>
</template>
```

## 🔧 Options

Nothing.
