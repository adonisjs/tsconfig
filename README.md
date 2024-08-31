# @adonisjs/tsconfig

<hr>
<br />

<div align="center">
  <h3>Base TSConfig files</h3>
  <p>TSConfig config files for AdonisJS (including Inertia) applications or AdonisJS packages.</p>
</div>

<br />

<div align="center">

[![npm-image]][npm-url] [![license-image]][license-url]

</div>

## Installation

Install the package from the npm registry.

```sh
npm i -D @adonisjs/tsconfig@beta

# Make sure also to install the following packages
npm i -D typescript ts-node-maintained @swc/core
```

## Usage

After installation, use one of the following base config files.

**For package development**

```json
// tsconfig.json
{
  "extends": "@adonisjs/tsconfig/tsconfig.package.json",
  "compilerOptions": {
    "rootDir": "./",
    "outDir": "./build"
  }
}
```

**For AdonisJS application**

```json
// tsconfig.json
{
  "extends": "@adonisjs/tsconfig/tsconfig.app.json",
  "compilerOptions": {
    "rootDir": "./",
    "outDir": "./build"
  }
}
```

**For client-side code inside AdonisJS application**

```ts
// resources/tsconfig.json
{
  "extends": "@adonisjs/tsconfig/tsconfig.client.json"
}
```

<div align="center">
  <sub>Built with ❤︎ by <a href="https://github.com/Julien-R44">Julien Ripouteau</a> and <a href="https://github.com/thetutlage">Harminder Virk</a>
</div>

[npm-image]: https://img.shields.io/npm/v/@adonisjs/tsconfig/latest.svg?style=for-the-badge&logo=npm
[npm-url]: https://www.npmjs.com/package/@adonisjs/tsconfig/v/latest 'npm'
[license-url]: LICENSE.md
[license-image]: https://img.shields.io/github/license/adonisjs/tsconfig?style=for-the-badge
