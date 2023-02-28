```
npx create-react-app . --template typescript
```

```
npm install eslint @typescript-eslint/parser @typescript-eslint/eslint-plugin --save-dev
```

```
npm install prettier eslint-config-prettier eslint-plugin-prettier --save-dev
```

- eslint-config-prettier: prettier와 충돌을 일으키는 eslint 규칙 비활성화 config(설정파일)
- eslint-plugin-prettier: eslint 규칙에 따라 작동하게 해주는 플러그인

```
npm init @eslint/config
```

```
npx eslint --cache .
```

```
npm install husky --save-dev
npx husky install
```

```
// package.json

  "scripts": {
    "postinstall":"husky install"
  },
```

```
npx husky add .husky/pre-commit "npm run format"
npx husky add .husky/pre-push "npm run lint"
```
