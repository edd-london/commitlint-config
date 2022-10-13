# EDD Commitlint Config

Our default export contains rules related to commits by following [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)
specifications.

## Prerequisites

`npm install npm@latest -g`

`npm install --global yarn`

## Installation

### install commitlint

`npm install --save-dev @commitlint/{cli,config-conventional}`

`yarn add @commitlint/{cli,config-conventional} -D`

### Install husky

`npm install husky --save-dev`

`yarn add husky --dev`

#### activate hooks

`npx husky install`

`yarn husky install`

### Add hook

`npx husky add .husky/commit-msg "npx --no -- commitlint --edit ${1}"`

### Hooks not running

- Ensure that you don't have a typo in your filename. For example, precommit or pre-commit.sh are invalid names. See Git hooks [documentation](https://git-scm.com/docs/githooks) for valid names.
- Check that git config core.hooksPath returns .husky (or your custom hooks directory).
- Verify that hook files are executable. This is automatically set when using husky add command but you can run `chmod +x .husky/<hookname>` to fix that.
- Check that your version of Git is greater than 2.9.

## Usage

- create a file called `.commitlintrc.json` in root directory of application where .git file is located.
- paste the following snippet <code>{<br/> &nbsp;&nbsp;extends: ['@eddlondon'];<br/>}</code>.

## Publish

run the following command <br/>

`yarn push-patch`

`npm run push-minor`

`yarn push-minor`

`npm publish access=public`
