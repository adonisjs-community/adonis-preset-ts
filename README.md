<div align="center">
  <img src="https://res.cloudinary.com/adonisjs/image/upload/q_100/v1558612869/adonis-readme_zscycu.jpg" width="600px">
</div>

<br />
<hr>

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
    "paths": {
      "App/*": [ "./app/*" ],
      "Contracts/*": [ "./contracts/*" ]
    }
  }
}
```