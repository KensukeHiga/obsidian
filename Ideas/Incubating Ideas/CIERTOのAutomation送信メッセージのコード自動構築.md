---
STATUS: 実行中
MVP_TIME: 7
tags:
  - LLM
---
# 組み合わせ


# 楽しそうなこと
伊芸さんから依頼があった。
「[[CIERTO Automation]]を使って、アセットがUPされたら[[slack]]に通知したい。
フォルダをUPしたときはフォルダ名とファイル名は分離して箇条書きにしたい。」
[[API]]の送信内容構築なので、たしかにエンジニアじゃないとかなりコストの高い依頼だった。
これを自動化できれば
- ユーザーの「機能が使えない」な不満を払拭
- サポートの対応時間削減
ができてとても良さそう。

[[CIERTO Automation]]マニュアルをAIに学習させて、送信したいメッセージをAIに伝えたら作ってくれないか。
↓
ちょっとやってみたけど、フォルダとファイルの区別の部分などで不十分なコードが提示された。
これを「不十分」と判断できる人じゃないと、スラックに送信してみて実現したいメッセージとの差分をAIに共有して修正させて
な流れになるのでやり取りに時間がかかる。
↓
そういった上手くいかなかった部分を補うドキュメントを学習させればいけるのか？