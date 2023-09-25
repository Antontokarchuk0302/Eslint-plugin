
> Official ESLint plugin for Vue.js

## :book: Documentation

Please refer to the [official website](https://eslint.vuejs.org).

## :anchor: Versioning Policy

This plugin follows [Semantic Versioning](https://semver.org) and [ESLint's Semantic Versioning Policy](https://github.com/eslint/eslint#semantic-versioning-policy).

## :newspaper: Releases

This project uses [GitHub Releases](https://github.com/SeniorDev1123/Vue-plugin/releases).


### Working With Rules

To see what an abstract syntax tree (AST) of your code looks like, you may use [AST Explorer](https://astexplorer.net). After opening [AST Explorer](https://astexplorer.net), select `Vue` as the syntax and `vue-eslint-parser` as the parser.

`vue-eslint-parser` provides a few useful parser services to help traverse the produced AST and access template tokens:

- `context.parserServices.defineTemplateBodyVisitor(visitor, scriptVisitor)`
- `context.parserServices.getTemplateBodyTokenStore()`

Be aware that depending on the code samples you write in tests, the `RuleTester` parser property must be set accordingly (this can be done on a test by test basis). 

