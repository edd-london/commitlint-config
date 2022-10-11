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

## Usage

- create a file called `.commitlintrc.json` in root directory of application where .git file is located.
- paste the following snippet <code>{<br/> &nbsp;&nbsp;extends: ['@eddlondon'];<br/>}</code>.

## Publish

run the following command <br/>

`npm run push-minor`

`yarn push-minor`
