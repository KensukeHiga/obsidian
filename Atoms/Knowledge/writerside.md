# ざっくり
### [[Docs as Code]] パイプライン

> 単一のオーサリング環境を使用するため、多様なツールを用意する必要はありません。組み込みの Git UI、統合ビルドツール、自動テスト、既製のカスタマイズ可能なレイアウトを使用することで、最も重視すべきドキュメントの内容に専念できます。

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
１つのInstanceが１つの製品ドキュメント。
別Instanceであっても、同一プロジェクトであれば任意のコンテンツをインスタンス間で再利用できる。
### Table of contents（目次）
目次 (TOC) はインスタンスの構造を表します。これは、タグを使用してツリー ファイルで定義されます `<toc-element>`
### Topics（要素）の保存場所
Instance下に作成したマークダウンファイルや画像などはInstanceに紐づくのではなく、添付画像のようにProject共通資産としてtopics配下に保存される。
![[スクリーンショット 2024-06-03 171518.png]]

# メリット
- Gitでバージョン管理、レビューができるので品質管理しやすい。
- Instance単位でMDファイルがまとまるので一元管理できる。
- リンクが相互に把握でき、リンク先の情報を変数として表示可能。
	- 仕様変更決定時の修正必要資料の漏れ防止
	- しかし2024年6月10日現在ではIntelliJの「X件の使用箇所（リンク）」のような表示はされず、ctrl+クリックで使用箇所が表示されるのみ。
	- 宣言箇所を削除するとリンク切れエラーは出してくれる。
- 自動チェックを設定可能