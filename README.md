# Vue 3 + TypeScript + Vite

## 環境建置
### Eslint + prettier配置
1. 安裝 eslint
   > npm i aslant

2. 初始化配置eslint
   > npx eslint —init

3. 選擇模式
   > To check syntax and find problems
      
   選擇語言
   > javascript

   選擇語言框架      
   > vue.js
   
   使用ts?
   > yes

   在哪裡運行(使用空白鍵選組兩個 Browser + Node)

   配置文件的格式
   > javascript

   現在就要安裝嗎？
   > yes

   哪個管理器     
   > npm 
      
4. 安裝完成後會自動產生(eslintrc.js)

5. 安裝vite-plugin-eslintnpm: 
   > npm i vite-plugin-eslint
6. 安裝 eslint-parser    
   > npm i  @babel/core

   > npm i  @babel/eslint-parser

7. 安裝prettier
   >  npm i prettier

   >  npm i eslint-config-prettier

   >  npm i eslint-plugin-prettier 


8. 配置 vite.config.js
```ts
  import eslintPlugin from 'vite-plugin-eslint'
  
  plugins: [
    vue(),
    eslintPlugin({
      include: [ 
         'src/**/*.js',
         'src/**/*.vue',
         'src/*.js',
         'src/*.vue'
      ]
   }),
  ]
```
9. 配置 .eslintrc.cjs

## 開啟

```
npm run dev
```

### 打包

```
npm build
```
