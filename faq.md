---
layout: post
title: FAQ
---

# よくある質問

## Q. エラーが発生して動かない！

エラーの原因には様々なケースがあります。こうすれば必ず直るという特効薬はありません。ただ、始めたばかりの人がつまずきやすいポイントとしては、以下のようなものがあります。

### 打ち間違いにご用心

スクリプトの中で使うクラス名、関数名、予約語の類は、大文字・小文字が異なるだけでエラーになります。一字一句間違えないように入力を行いましょう。Unityに付属のスクリプトエディターを使う場合、あらかじめ定義された語をカラーリングして表示してくれます。正確に入力したつもりなのにカラーが変わらない場合は、何か打ち間違えている可能性が高いです。カラーが変わるまで確認しましょう。

### プレハブのドラッグ＆ドロップを忘れない

プレハブを使うようになってくると間違いやすいミスとして、プレハブをセットするつもりだった変数をnullのまま放置してしまい、それが原因でエラーになってしまうということがあります。変数をnullのまま放置することというのはほぼあり得ないので、見つけたら必ず対処しましょう。

## Q. 正常に動いているけどエラーが出続ける / 1回の入力で2回効果が出る

スクリプトが余計な所に追加されている可能性があります。追加した覚えのない場所にスクリプトが追加されていないかどうか、全体をチェックしてみましょう。
