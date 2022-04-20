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
重要的文件就是
  1 -> .vscode/setting.json
  2 -> .eslintrc.js
  3 -> package.json
```
```
.eslintrc.js 这个文件夹里面写了一些配置，你可以在这里面修改，也可以直接在rules中覆盖
```
For example:
```json
{
  "rules": {
    "no-console": "off"
  }
}
```


## Usage
### Clone --- 直接 clone 使用，不解释。

```bash
// 直接使用 纯净的本仓库开搞。
npx degit https://github.com/TTiip/eslint-template-utils xxx
```

