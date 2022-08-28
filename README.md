# TODO
- mongoose
- swaggerからAPIのテストもしたい
- - 認証の問題

# コマンド
### swagger定義ファイルを一つにまとめる
```
npx swagger-cli bundle -o swagger/.build/out.yml -t yaml swagger/index.yml 
```
### swagger-uiを立ち上げる
```
npx swagger-ui-watcher swagger/.build/out.yml
```
### swaggerからTypeScriptの型定義を生成する
```
npx sta -p swagger/.build/out.yml -o types -n out.ts
```