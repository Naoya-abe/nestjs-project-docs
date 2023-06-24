# 🗄️ ディレクトリ構造

```
docs                 # Documents

prisma               # Prisma関連のファイル群。マイグレーションファイル・スキーマ・シード実行ファイル

src                  # アプリケーションのメインディレクトリ
|
+-- @generated
|       |
|       +-- prisma-nestjs-graphql    # Prismaが生成した型定義ファイル群（基本的に編集しない）
|
+-- (module name)
|       |
|       +-- dto        # DataTransferObjectを定義したファイル群（必要な場合）
|       |
|       +-- guards     # 認証・認可ガードを定義したファイル群（必要な場合）
|       |
|       +-- strategies # 認証・認可戦略を定義したファイル群（必要な場合）
|       |
|       +-- types      # 各処理の型定義ファイル群（必要な場合）
|       |
|       +-- (module name).controller.ts
|       |
|       +-- (module name).module.ts
|       |
|       +-- (module name).resolver.ts
|       |
|       +-- (module name).service.ts
|
+-- utils            # ユーティリティファイル群
|
+-- app.module.ts    # アプリケーション全体で使用されるグローバルな機能や設定を定義する（ルートモジュール）
|
+-- main.ts          # プログラムが実行される際に最初に呼び出されるファイル（エントリーポイント）
|
+-- schema.gql       # GraphQLが自動生成したgqlスキーマファイルが入っている（基本的に編集しない）

test                 # e2eテスト、インテグレーションテスト
```
