# EDD Commitlint Config

Our default export contains rules related to commits by following [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)
specifications.

## Prerequisites

`npm install npm@latest -g`

`npm install --global yarn`

## Installation

`npm i @edd/commitlint-config`
`yarn add @edd/commitlint-config`

## Usage

- create a file called `.commitlintrc.json` in root directory of application
- paste the following snippet <code>{<br/> &nbsp;&nbsp;extends: ['@eddlondon'];<br/>}</code>.

## Publish

run the following command <br/>

`npm run push-minor`

`yarn push-minor`
