# Adonis Preset Typescript

This module contains the base config files **(recommended by the core team)** for `typescript` and `tslint` to be extended by your AdonisJs typescript projects.

## Usage
Install the package from npm registry as follows

```sh
npm i -D adonis-preset-ts

# yarn
yarn add -D adonis-preset-ts
```

and then setup your config files to extend the base config

**tsconfig.json**

```json
{
  "extends": "./node_modules/adonis-preset-ts/tsconfig",
  "compilerOptions": {
    "types": [
      "@adonisjs/core"
    ],
    "paths": {
      "App/*": [ "./app/*" ],
      "Contracts/*": [ "./contracts/*" ]
    }
  }
}
```

**tslint.json**

```json
{
  "extends": [
    "adonis-preset-ts/tslint"
  ],
  "rules": {}
}
```