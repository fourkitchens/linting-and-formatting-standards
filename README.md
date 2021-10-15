## Tools

### Local

- [nvm](https://github.com/nvm-sh/nvm): Define the supported node version in a `.nvmrc` file, and then type `nvm use` into the terminal to ensure a consistent developer experience across environments. (The `use` command [can be automated](https://github.com/nvm-sh/nvm#automatically-call-nvm-use) per environment as well)
  - Files
    - `.nvmrc`
- Eslint: Javascript
- Stylelint: CSS
- [Prettier](https://prettier.io/docs/en/index.html): Opinionated code formatter with support for many file types. You can configure your [editor to use prettier](https://prettier.io/docs/en/editors.html) so that code is formatted on save, for example.
  - Files:
    - `.prettier.json`
    - `.prettierignore`
  - Integrations:
    - [eslint-config-prettier](https://github.com/prettier/eslint-config-prettier): Configure Prettier to play nice with eslint
      - Affects file: `.eslintrc.json`
    - [eslint-plugin-prettier](https://github.com/prettier/eslint-plugin-prettier) Runs Prettier as an ESLint rule
      - Affects file: `.eslintrc.json`
    - [stylelint-config-prettier](https://github.com/prettier/stylelint-config-prettier): Configure Prettier to play nice with stylelint
      - Affects file: `.stylelintrc.json`
- [Husky](https://github.com/typicode/husky): Performs linting/formatting automatically around git commands. e.g. `git commit`, `git push`, etc.
- [lint-staged](https://github.com/okonet/lint-staged): Used by Husky to lint only staged (changed) files, as opposed to the whole code base (Note: The whole code base will be linted later, as a check for anything that was forced through, etc. This mostly improves the day-to-day developer experience.)
- [Commit Lint](https://commitlint.js.org/#/): Verifies commit messages follow the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) standard for many reasons. One being that it automates release notes, and semantic version bumping.

### CI (Build Environment)

- [semantic-release](https://github.com/semantic-release/semantic-release) or [standard-version](https://github.com/conventional-changelog/standard-version) for automated version bumping (based on commit messages.)
