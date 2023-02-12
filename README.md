# ...？(´・ω・｀)
IntelliJ系のIDEでTypeScriptを実行する設定例

# 環境準備
Node.jsが必要  
nodenvが入っていればいい感じに動くはず

# それぞれの説明
## start
### 説明
npmで実行する
```shell
npm start
```
と同じ
### 事前準備
```json
{
  "scripts": {
      "start": "tsc && node dist/helloWorld.js"
  },
  "devDependencies": {
    "typescript": "^10.9.1"
  }
}
```
```shell
npm install
```

## helloWorld.ts
### 説明
ts-nodeを利用してTypeScriptをNode.jsで直接動かす
### 事前準備
```json
{
  "devDependencies": {
    "ts-node": "^10.9.1"
  }
}
```
```shell
npm install
```

## helloWorld.js
### 説明
実行前にTypeScriptのコンパイルを行う設定がされている  
最初の1回はファイルがないため設定を修正しなさいといわれるため、無視して実行する必要がある
### 事前準備
```shell
npm install -g typescript
```
