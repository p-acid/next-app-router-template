# Next.js Template for Quick Development

## Features

- Default settings for development with next.js app router
- Workflow for notifications of PR by Telegram
  - PR created
  - PR reviewed
- Utils for creating custom react query hook

## Commands

```sh
# init shadcn
npx shadcn-ui@latest init
npx shadcn-ui@latest add [ui-name]

# eslint plugin
yarn add -D eslint-config-prettier eslint-plugin-react eslint-plugin-tailwindcss

# import orders
yarn add -D @ianvs/prettier-plugin-sort-imports

# pre-commit, commit-msg
yarn add -D husky lint-staged @commitlint/config-conventional @commitlint/cli
yarn husky install
npx husky add .husky/pre-commit "yarn lint-staged"
echo "module.exports = { extends: ['@commitlint/config-conventional'] };" > commitlint.config.js
yarn husky add .husky/commit-msg "yarn commitlint --edit $1"
```
