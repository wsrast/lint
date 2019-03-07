# airbnb-prettier-eslint
Setup files for eslint, editorconfig and prettier. For bootstrapping new JS projects.

## Setting up Airbnb code config
from: https://blog.echobind.com/integrating-prettier-eslint-airbnb-style-guide-in-vscode-47f07b5d7d6a

reference: https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb

### New Hotness Way

This new structure allows you to use a single command to do everything. The -Y flag will automatically choose Yarn as the package installer.

```
npm install-peerdeps --dev -Y @wsrast/airbnb-prettier-eslint eslint-config-airbnb
```

### Manual Way

```
yarn add --dev eslint prettier husky lint-staged eslint-config-prettier eslint-plugin-prettier eslint-plugin-react-hooks

npx install-peerdeps --dev eslint-config-airbnb
```
(opt to use yarn for install)

If you're going against convention and adding this to the top level of a Yarn Workspace, use the following npx command instead.

```
npx install-peerdeps --dev eslint-config-airbnb --extra-deps -W
```