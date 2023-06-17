# Eslint Config JS Stack

ESLint and Prettier configuration for JavaScript stack, providing comprehensive and optimized setups for React and Node.js projects.

## Plugins

This configuration utilizes the following ESLint plugins:

- [@typescript-eslint/eslint-plugin](https://www.npmjs.com/package/@typescript-eslint/eslint-plugin)
- [@typescript-eslint/parser](https://www.npmjs.com/package/@typescript-eslint/parser)
- [eslint-plugin-jsx-a11y](https://www.npmjs.com/package/eslint-plugin-jsx-a11y)
- [eslint-plugin-prettier](https://www.npmjs.com/package/eslint-plugin-prettier)
- [eslint-plugin-react](https://www.npmjs.com/package/eslint-plugin-react)
- [eslint-plugin-react-hooks](https://www.npmjs.com/package/eslint-plugin-react-hooks)
- [prettier](https://www.npmjs.com/package/prettier)

## Installation

```bash
npm install eslint-config-js-stack --save-dev
```

## Usage

To use the ESLint and Prettier configurations provided by eslint-config-js-stack, add the following to your project's ESLint configuration file:

```json
{
  "extends": "eslint-config-js-stack/react"
  // "extends": "eslint-config-js-stack/node"
}
```
For React projects, use "eslint-config-js-stack/react" in the "extends" array.
For Node.js projects, use "eslint-config-js-stack/node" in the "extends" array.

## Overriding ESLint Configuration

You can add or override any ESLint configuration rules by creating your own .eslintrc.json file in your project and extending the eslint-config-js-stack configuration. Here's an example:

```json
{
  "extends": [
    "eslint-config-js-stack/react",
    "my-custom-config"
  ],
  "rules": {
    "my-custom-rule": "error"
  }
}
```

In the example above, we extend both the eslint-config-js-stack/react configuration and another custom configuration called "my-custom-config". We can also add or override specific ESLint rules in the "rules" object.

## Ignoring Files

To enhance the integration of ESLint and Prettier in your project, it's recommended to add .eslintignore and .prettierignore files to exclude certain files and directories from version control and code formatting. You can use the following examples on my [gist](https://gist.github.com/raphaeljcm/cf439ddd5bcab27a0a0588d071696d75) as a starting point