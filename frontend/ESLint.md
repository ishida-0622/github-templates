# セットアップ

`package.json`があるディレクトリで以下のコマンドを実行

```bash
npm i -D eslint eslint-config-prettier eslint-plugin-import eslint-plugin-unused-imports husky lint-staged prettier
```

TypeScript の場合は以下を追加でインストール

```bash
npm i -D @typescript-eslint/eslint-plugin @typescript-eslint/parser
```

React.js の場合は以下を追加でインストール

```bash
npm i -D eslint-plugin-react
```

Next.js の場合は以下を追加でインストール

```bash
npm i -D eslint-config-next
```

`package.json`に以下を追記

```json
  "lint-staged": {
    "*.{js, jsx, ts, tsx, json}": "eslint --fix && prettier --write"
  },
```
