# ClearTrace Prettier configuration

A [Prettier](https://prettier.io) configuration for consistency in [ClearTrace](https://cleartrace.io) projects

## Compatible Prettier version

This version of the configuration complements **Prettier 2.2.1**. Pairing this configuration with a different version of Prettier may result in inconsistent style.

[Prettier's installation documentation](https://prettier.io/docs/en/install.html) recommends:

<blockquote>
Install an exact version of Prettier locally in your project. This makes sure that everyone in the project gets the exact same version of Prettier. Even a patch release of Prettier can result in slightly different formatting, so you wouldn’t want different team members using different versions and formatting each other’s changes back and forth.
</blockquote>

## Setup

1. Make sure the exact, correct, complementary version of Prettier is installed.

1. Install this package.

   ```sh
   npm install @swytchio/prettier-config
   ```

1. Instruct Prettier to use the configuration from this package.

   Remove any preexisting Prettier configuration, but preserve `.prettierignore`.

   In `package.json`:

   ```json
   "prettier": "@swytchio/prettier-config"
   ```

1. Commit this configuration update without applying the new style rules.

1. Run `npx prettier --write .` to apply the new style rules.

1. Commit the Prettier-rewritten files.

   It is courteous to create a dedicated PR for these automated changes.
