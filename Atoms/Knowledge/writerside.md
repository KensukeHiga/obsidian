# ざっくり
### [[Docs as Code]] パイプライン
単一のオーサリング環境を使用するため、多様なツールを用意する必要はありません。組み込みの Git UI、統合ビルドツール、自動テスト、既製のカスタマイズ可能なレイアウトを使用することで、最も重視すべきドキュメントの内容に専念できます。

```cardlink
url: https://www.jetbrains.com/ja-jp/writerside/
title: "Writerside - JetBrains が提供する新しい技術文書作成環境。"
description: "Writerside は JetBrains が提供する新しい技術文書オーサリングおよびパブリッシング環境です。"
host: www.jetbrains.com
favicon: https://www.jetbrains.com/favicon.ico?r=1234
image: https://resources.jetbrains.com/storage/products/writerside/img/meta/preview.png
```



# メモ
## 用語
### Project
全ての要素を含み管理する。コードでいうところのProjectと大体一緒。
### Instance
1つのドキュメント。このInstance単位で目次が生成され、ドキュメントのタイトルにはInstance名が入る。
Googleドキュメントの１ファイルがInstanceにあたる。
別Instanceであっても、同一プロジェクトであれば任意のコンテンツをインスタンス間で再利用できる。
### Table of contents（目次）
目次 (TOC) はインスタンスの構造を表します。これは、タグを使用してツリー ファイルで定義されます `<toc-element>`
