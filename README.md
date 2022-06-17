Harker Robotics apps use [prettier](https://prettier.io) to enforce a standardized code style across codebases. The `@harker-robo/prettier-config` NPM package defines the formatting rules.

## Installation
Install [prettier](https://www.npmjs.com/package/prettier) and the configuration package.

    npm i --save-dev prettier @harker-robo/prettier-config

## Usage
1. Add the `prettier` key to package.json
```jsonc
// package.json
{
    // ...
    "prettier": "@harker-robo/prettier-config"
}
```

2. Add the formatting script to package.json.
```jsonc
// package.json
{
    // ...
    "scripts": {
        // ...
        "format": "npx prettier . -w"
    }
}
```

3. Run the formatter.
```
npm run format
```

## Links
* [Ignoring files](https://prettier.io/docs/en/ignore.html)
* [GitHub integration](https://github.com/marketplace/actions/prettier-action)
* [Editor integration](https://prettier.io/docs/en/editors.html)
* [Overriding configuration](https://prettier.io/docs/en/configuration.html) (not recommended)
