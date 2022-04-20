# eslint-template-utils

## 特别感谢 [antfu](https://github.com/antfu) 大佬的 [eslint](https://github.com/antfu/eslint-config) 配置

- Single quotes, no semi
- Auto fix for formatting (aimed to be used standalone without Prettier)
- TypeScript, Vue, React out-of-box
- Lint also for json, yaml, markdown
- Sorted imports, dangling commas for cleaner commit diff
- Reasonable defaults, best practices, only one-line of config

## Options
```
.eslintrc.js 这个文件夹里面写了一些配置，你可以在这里面修改，也可以直接在rules中覆盖
```
For example:
```json
{
  "extends": "@antfu",
  "rules": {
    "no-console": "off"
  }
}
```


## Usage

> 方案一
### Clone --- 直接 clone 使用，不解释。

```bash
// 直接使用 纯净的本仓库开搞。
npx degit https://github.com/TTiip/eslint-template-utils xxx
```

> 方案二 --- 安装大佬的库自己配置。
### Install --- 安装依赖继续配置。
```
// 安装依赖，yarn、pnpm、npm、cnpm愿意用哪个用哪个。
yarn add -D eslint @antfu/eslint-config
```

### Config `.eslintrc.js` --- 配置这里改。

```json
{
  "extends": "@antfu"
}
```

### Add script for package.json --- 在 package.json 中添加脚本，一键修复。

For example:

```json
{
  "scripts": {
    "lint": "eslint .",
    "lint:fix": "eslint . --fix"
  }
}
```

### Config VS Code auto fix --- 也可以配置保存自动修复

Create `.vscode/settings.json`

```json
{
  "prettier.enable": false, // 关闭 prettier 自动修复
  "editor.codeActionsOnSave": { // 保存时自动修复
    "source.fixAll.eslint": true // 打开 eslint 自动修复
  }
}
```

## License

MIT
