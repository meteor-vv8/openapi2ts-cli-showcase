# OpenApi2TS-CLI

OpenAPI 3.0 の仕様書(JSON / YAML)から、TypeScriptの型定義とfetchベースのAPIクライアントコードを自動生成するCLIツールです。

📦 購入はこちら: https://meteor01.gumroad.com/l/erogi

## このリポジトリについて

これは製品の紹介ページです。実装のソースコードは購入者向けに非公開で管理されており、このリポジトリには含まれていません。仕様や使い方の確認、Star・Issueでのフィードバックにご利用ください。

## 特徴

・OpenAPI 3.0のcomponents.schemasからTypeScriptのinterface/typeを自動生成

・$ref、allOf(交差型)、oneOf/anyOf(合併型)、enum、nullable、additionalPropertiesに対応

・各エンドポイントごとに、型付きのfetchラッパー関数を自動生成

・パスパラメータ、クエリパラメータ、リクエストボディを引数として型付け

・外部ランタイム依存なし(生成コードは標準のfetchのみを使用)

・JSON / YAMLどちらの仕様書にも対応

## 使い方(イメージ)

```
openapi2ts generate <OpenAPI仕様書のパス> --out <出力ディレクトリ> [--base-url <URL>]
```

実行すると、指定した出力ディレクトリに型定義(types.ts)とAPIクライアント関数(client.ts)が生成されます。

## ライセンス概要

本ソフトウェアは購入者向けの買い切りライセンスです。

・許可: 購入者本人、または所属組織内での個人・商用利用

・禁止: 第三者への再配布・転売、別の有償デジタル商品としての再パッケージ

詳細・購入は https://meteor01.gumroad.com/l/erogi からご確認ください。
