Quick and easy repo template for creating a web extension.

What did I do to make this?

- Set up .gitignore using some of [GitHub's presets](https://github.com/github/gitignore)
- Created empty package.json (`{}`; you can do `npm init` if you prefer)
- Installed eslint and prettier
  - `npm add -D eslint` (or `npx install-peerdeps --dev eslint-config-airbnb` or `npx install-peerdeps --dev eslint-config-airbnb-base`)
  - `npm install -D prettier`
  - `npm install -D eslint-config-prettier` (possibly optional without a config, but good to know about)
- Added basic config files for:
  - editorconfig
  - eslint (`"es2022": true` allows top-level await, `??=`, etc)
  - prettier (my `printWidth` and `quoteProps`settings are kind of opinionated)
- Added eslint and prettier scripts
- Added basic automatic eslint + prettier GitHub workflow

Plus:

- Installed web-ext (`npm i -D web-ext`) and added package.json config
- Added web-ext scripts
- Created example MV2/MV3 web extension with one content script
  - note: at time of writing, in MV3, Firefox and Chrome have different formats for background scripts/pages
