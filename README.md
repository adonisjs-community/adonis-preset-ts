<div align="center">
  <img src="https://res.cloudinary.com/adonisjs/image/upload/q_100/v1558612869/adonis-readme_zscycu.jpg" width="600px">
</div>

<br />

<div align="center">

[![npm-image]][npm-url] ![][typescript-image] [![license-image]][license-url] [![synk-image]][synk-url]

</div>

<br />

# Adonis Preset Typescript

This module contains the base config files **(recommended by the core team)** for `typescript` to be extended by your AdonisJS typescript projects.

## Usage
Install the package from npm registry as follows

```sh
npm i -D adonis-preset-ts

# yarn
yarn add -D adonis-preset-ts
```

and then setup your config file to extend the base config

**tsconfig.json**

```json
{
  "extends": "./node_modules/adonis-preset-ts/tsconfig",
  "compilerOptions": {
    "types": [
      "@adonisjs/core"
    ],
    "outDir": "./build",
    "rootDir": "./",
    "paths": {
      "App/*": ["./app/*"],
      "Config/*": ["./config/*"],
      "Contracts/*": ["./contracts/*"],
      "Database/*": ["./database/*"]
    }
  },
  "include": ["**/*"],
  "exclude": ["node_modules", "build"]
}
```

<div align="center">
  <sub>Built with ❤︎ by <a href="https://github.com/thetutlage">Harminder Virk</a>
</div>

[npm-image]: https://img.shields.io/npm/v/adonis-preset-ts/latest.svg?style=for-the-badge&logo=npm
[npm-url]: https://www.npmjs.com/package/adonis-preset-ts/v/alpha "npm"

[typescript-image]: https://img.shields.io/badge/Typescript-294E80.svg?style=for-the-badge&logo=typescript

[license-url]: LICENSE.md
[license-image]: https://img.shields.io/github/license/adonisjs-community/adonis-preset-ts?style=for-the-badge

[synk-image]: https://img.shields.io/snyk/vulnerabilities/github/adonisjs-community/adonis-preset-ts?label=Synk%20Vulnerabilities&style=for-the-badge
[synk-url]: https://snyk.io/test/github/adonisjs-community/adonis-preset-ts?targetFile=package.json "synk"
