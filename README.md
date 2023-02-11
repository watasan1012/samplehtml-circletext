# samplehtml-circletext

## .gitignoreファイルの作成

```sh
% echo ".DS_Store" >> .gitignore
```

### npm でインストールされたパッケージ名のフォルダ配下をアップロードしない様に記載する

- ディレクトリを指定する場合

node_modules/ を、.gitignoreファイルに記述する

## コードを綺麗にしよう

node.jsと、npm が必要です

- package.jsonの作成

```sh
% npm init -y
```

### stylelintとその基本設定ファイルをインストール

```sh
% npm install --save-dev stylelint stylelint-config-standard
```

### stylelintの設定ファイルを作成する

```sh
% touch .stylelintrc.json
```

### .stylelintrc.jsonの中身の設定

```json
{
  "extends": "stylelint-config-standard"
}
```

### stylelintを実行してみよう

```sh
% npx stylelint "**/*.css"
```

"**/*.css"の部分はパスを設定する

```sh
% npx stylelint "*.css"
```

ルールによって報告された問題を、可能な限り自動的に修正します。

```sh
% npx stylelint --fix "**/*.css"
```

```sh
% npx stylelint --fix "*.css"
```
