## Babel

Babel loader with `@babel/preset-env` is already configured for you.

Create a `babel.config.js` file on your project root like:

```js
module.exports = {
    presets: [
        [
            '@babel/preset-env',
            {
                bugfixes: true,
                modules: false,
                useBuiltIns: false,
                targets: {
                    // browsers: ['> 2%', 'not dead']
                }
            }
        ]
    ],
    plugins: [
        // Your babel plugins
    ],
}
```

You can remove the `babel` property from your `package.json`.

* [Read more](https://babeljs.io/docs/en/config-files)
