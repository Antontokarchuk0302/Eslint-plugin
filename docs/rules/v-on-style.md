# enforce `v-on` directive style (v-on-style)

- :white_check_mark: The `"extends": "plugin:vue/recommended"` property in a configuration file enables this rule.
- :wrench: The `--fix` option on the [command line](http://eslint.org/docs/user-guide/command-line-interface#fix) can automatically fix some of the problems reported by this rule.

This rule enforces `v-on` directive style which you should use shorthand or long form.

## :book: Rule Details

:-1: Examples of **incorrect** code for this rule:

```html
<template>
    <div>
        <div v-on:click="foo"></div>
    </div>
</template>
```

:+1: Examples of **correct** code for this rule:

```html
<template>
    <div>
        <div @click="foo"></div>
    </div>
</template>
```

:-1: Examples of **incorrect** code for this rule with `"longform"` option:

```html
<template>
    <div>
        <div @click="foo"></div>
    </div>
</template>
```

:+1: Examples of **correct** code for this rule with `"longform"` option:

```html
<template>
    <div>
        <div v-on:click="foo"></div>
    </div>
</template>
```

## :wrench: Options

- `"shorthand"` (default) ... requires using shorthand.
- `"longform"` ... requires using long form.
