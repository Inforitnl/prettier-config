# @inforit/prettier-config

Inforit's preferred prettier configuration.

<!-- toc -->

- [Installation](#installation)
- [Configuration](#configuration)
  - [package.json](#packagejson)
  - [.prettierrc.js](#prettierrcjs)

<!-- tocstop -->

## Installation

Simply install the package with npm:

`npm install --save-dev @inforit/prettier-config`

## Configuration

Configuring your project to use `@inforit/prettier-config` can be done in several ways.  
The easiest is the [package.json](#packagejson) solution, the most extensible is the [.prettierrc.js](#prettierrcjs) version.

### package.json

Simply add a "prettier" key with the package name:

```json
{
  "prettier": "@inforit/prettier-config"
}
```

### .prettierrc.js

This solution requires you to put a `.prettierrc.js` file at the root of your project with the following code:

```js
module.exports = {
  ...require("@inforit/prettier-config"),
  // optional overrides:
  jsxBracketSameLine: true
};
```
