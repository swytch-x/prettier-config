# Contributing to the ClearTrace Prettier configuration

## How to restore after checkout

```sh
npm install
```

## How to check style

```sh
npx prettier --check .
```

or to check and automatically fix:

```sh
npx prettier --write .
```

## How to target a new version of Prettier

1. Specify the desired version of Prettier in:

   - `package.json`'s `devDependencies` and `peerDependencies`
   - the _Compatible Prettier version_ section of the [readme](README.md)

1. Run: `npm install`

1. Increment the major version of this package in `package.json`'s `version` property.

1. Commit these changes.

1. Apply the new style to this repository.

   ```sh
   npx prettier --write .
   ```

1. Commit the automated style changes if any were produced.

   It is courteous to create a dedicated PR for these automated changes.

## How to publish

These processes are currently manual, because these are early iterations of this package.

1. Appropriately increment the version in `package.json`.

   If the changes alter the style, including targeting a different version of Prettier, increment the major version.

2. Create a PR and obtain approval.
3. Merge to `main`.
4. Pull the latest `main`.
5. Run `npm install`.
6. Run `npm publish`.
