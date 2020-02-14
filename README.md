# GitMojo

[![NPM version][npm-version-img]][npm-url]

**Replace tags into your commit messages by emoji symbols**

## Requirements

- NodeJS v12.13.1
- [Husky v4.2.3](https://www.npmjs.com/package/husky)

## Install

Gitmojo need to be installed globally

```bash
yarn global add gitmojo
# or npm install gitmojo -g
```

## Initialize Gitmojo in your project

```bash
cd  my-project
gitmojo init
```

Edit `.gitmojorc.json` to fit your needs

## Husky's hook configuration

Update `Husky's` configuration with `prepare-commit-msg` hook

```
{
  "husky": {
    "hooks": {
      "prepare-commit-msg": "gitmojo"
    }
  }
}
```

## Defaults emojis

See [GITMOJO.md](./GITMOJO.md)

## TODOS

- [] check if Husky package is installed
- [] debug with windows EOL

[npm-url]: https://npmjs.org/package/gitmojo
[npm-version-img]: http://img.shields.io/npm/v/gitmojo.svg?style=flat-square
