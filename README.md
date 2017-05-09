# @detroit-labs/tslint-config

[![npm version](https://badge.fury.io/js/%40detroit-labs%2Ftslint-config.svg)](https://badge.fury.io/js/%40detroit-labs%2Ftslint-config)
[![Build Status](https://travis-ci.org/detroit-labs/tslint-config.svg?branch=master)](https://travis-ci.org/detroit-labs/tslint-config)
[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
[![Sponsored by Detroit Labs](https://img.shields.io/badge/Sponsor-Detroit%20Labs-000000.svg)](https://www.detroitlabs.com/open-source)

[TSLint](https://github.com/palantir/tslint/) configurations used in Detroit Labs' TypeScript projects

### Installation

```sh
$ yarn add @detroit-labs/tslint-config --dev
```

### Usage

To use the lint configuration with the default preset, use configuration inheritance via the `extends` keyword.
Here's a sample configuration where `tslint.json` lives adjacent to your `node_modules` folder:

```js
{
  "extends": ["@detroit-labs/tslint-config"],
  "rules": {
    // override rules here
    "semicolon": false
  }
}
```

To lint all TypeScript files in the `src/` directory, for example, run `tslint -c tslint.json 'src/**/*.{ts,tsx}'`.

### Development

#### Note

This project uses [semantic-release](https://github.com/semantic-release/semantic-release) for fully automated NPM package publishing. **Instead of using `git commit`, please use `yarn commit` and follow the prompts for entering a conventional changelog message.** This is crucial for letting tools manage package publishing and semantic versioning. :robot: Please see [this blog post](http://devboosts.com/2017/03/28/conventional-commits/) for a run through of the tooling used in this repo. If you are using GitHub Desktop to commit to this repo, please refer to the [AngularJS Git Commit Message Conventions](https://docs.google.com/document/d/1QrDFcIiPjSLDn3EL15IJygNPiHORgU1_OOAqWjiDU5Y/preview) (or use the command-line to commit :nerd_face:).

#### Workflow

* Install dependencies and commit hooks with `yarn install`
* Make changes to the TSLint configuration(s)
* Stage changes - `git add .`
* Create a conventional commit - `yarn commit`
* Push to GitHub and open a pull request

### Changelog

See the GitHub [release history](https://github.com/detroit-labs/tslint-config/releases).
