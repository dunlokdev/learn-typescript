## Setup Typescript
**Cài đặt Typescript**
```bash
nvm use 18.15.0

# using yarn
yarn --dev add typescript ts-node ts-lib @types/node # install typescript in local

```
> Lưu ý: Khi cài local thì vói các lệnh `tsc` `ts-node` cần phải thêm npx

```bash
npx tsc index.ts # biên dịch file index.ts sang index.js

npx ts-node index.ts # biên dịch ra run file index.ts
```

**Config format with Prettier tại:**
> https://prettier.io/playground

**Setup JEST test**
```bash
# using yarn
yarn add --dev jest typescript ts-jest @types/jest
yarn ts-jest config:init
```

**Khởi tạo file tsconfig.json mặc định**
```bash
tsc --init
```

```json
{
  "arrowParens": "always",
  "bracketSameLine": false,
  "bracketSpacing": true,
  "embeddedLanguageFormatting": "auto",
  "htmlWhitespaceSensitivity": "css",
  "insertPragma": false,
  "jsxSingleQuote": false,
  "printWidth": 100,
  "proseWrap": "preserve",
  "quoteProps": "as-needed",
  "requirePragma": false,
  "semi": true,
  "singleAttributePerLine": false,
  "singleQuote": true,
  "tabWidth": 2,
  "trailingComma": "es5",
  "useTabs": false,
  "vueIndentScriptAndStyle": false,
  "parser": "typescript"
}
```
## Config set Unrestricted mode on Windows
Open powershell with role administrator (Click mouse right -> Select run as administrator)

Chạy lệnh:

``` bash
get-ExecutionPolicy

#  "Restricted"
```

Tiếp tục chạy lệnh này để set `Unrestricted` :

``` bash
set-ExecutionPolicy Unrestricted
```
- Chọn phím khớp với option "Set to All" -> Enter

Cuối cùng để kiểm tra lại (sẽ được set lại là `Unrestricted`)

```bash
 get-ExecutionPolicy
```