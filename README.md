# eslint-config-trybe

ESLint shared configs used by projects from the Fundamentals, Front-end and Back-end modules

## Installation

Instructions should be the same for all three packages, with the only difference being the package
names.

These are the package names for each module:

- Fundamentals: `eslint-config-trybe-fundamentals`
- Front-end: `eslint-config-trybe-frontend`
- Back-end: `eslint-config-trybe-backend`

Once you've chosen a package, install it with:

```shell
$ npm i eslint-config-trybe-fundamentals
```

## Usage

Extend the chosen config on the `.eslintrc.json` of the project:

```json
{
  "extends": "trybe-fundamentals"
}
```

## Rules

Each package defines a set of ESLint rules judged appropriate for the given module. To see the rules
defined by each package, go to the [packages](./packages) folder and, inside the folder for the
desired package, open `config.json`

## Creating new packages

To create a new package, create its folder inside the `packages` folder and create a new NodeJS
package (using plain old `npm init`) inside it.

The config file should be named `config.json`, and this should be the entrypoint of the package.

The folder name should be everything that comes after `eslint-config-trybe` in the package name. So,
for `eslint-config-trybe-new-module`, the package folder should be called `new-module`.

## Publishing

This is a monorepo managed by [Lerna](https://github.com/lerna/lerna). You should read Lerna's docs
before publishing.

The versioning mode is `independent`.

To publish changed packages, simply run:

```shell
$ npx lerna publish
```
