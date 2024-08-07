# TS Config

This repository provides pre-configured TypeScript settings to simplify the setup of TypeScript and React projects. These configurations have been carefully crafted to optimize development, ensuring best practices and code quality standards from the start.

## How to use?

1. Before installing the configuration package, ensure that `typescript` is already installed in your project. If it is not, enter the following command in your terminal:

```bash
# NPM
npm install typescript@latest -D

# Yarn
yarn add typescript@latest -D

# PNPM
pnpm add typescript@latest -D
```

2. After installing typescript, you can run the following command to install the configuration package in your project.

```bash
# NPM
npm install @lucasaugustsof/ts-config -D

# Yarn
yarn add @lucasaugustsof/ts-config -D

# PNPM
pnpm add @lucasaugustsof/ts-config -D
```

3. Now, to use the configurations, create a `tsconfig.json` file at the root of your project and add the `extends` property to extend the desired configuration.

```json
{
  "extends": "@lucasaugustsof/ts-config/base.json"
}
```

```json
{
  "extends": "@lucasaugustsof/ts-config/react.json"
}
```

**Note:** It is important to mention that the React configuration already extends the base configuration by default.

4.	Your project is now set up with the predefined configurations. If you want to add or override any properties, it’s simple! Here is an example:

```json
{
  "extends": "@lucasaugustsof/ts-config/base.json",
  "compilerOptions": {
    "strictNullChecks": false
  }
}
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.