---
title: "Cloud Native 読書会第7回 runc"
date: 2021-05-19T20:00:00+09:00
draft: false
---
# はじめに
なおBlogs自分の日常のメモになります。

こんにちは以前にwantedlyの大坪さんの紹介で参加しました。

こちらから当日の内容は見ることができます。

https://zenn.dev/potsbo/scraps/f6bad62e1ac6ac


# 本文
runcって言葉はあまり聴き馴染みがない人が多いのではないでしょうか？

すくなくてもエンジニアとしてdockerなどをさわっていると無意識に触っているケースが非常に多いです。

dockerの簡易な歴史のがこちらにまとまっております。

https://eng-blog.iij.ad.jp/archives/1478

もともとdockerはエンジンとランタイムが同じなまえでした。

しかしインターフェースと中のランタイムをわける動きが出始めました。理由としてはもともとモジュールとして分離しており、汎用性をあげることが背景にあります。

Kubernetesもなどのコンテナオーケストレーションなどでも内部ではruncなどが扱いたいため、APIとしての提供が始まるのは無理もないですね。

そしてruncはもっともレイヤーが低い low level runtimeと呼ばれております。

ここらは非常におもしろく

日本製のコンテナランタイムのハコニワ https://github.com/haconiwa/haconiwa があったり
上記は多分OCIには準拠してないはずです。なのでKuberのruntimeには使えないかもしれないです。

Googleが作っているセキュアコンテナのgVisorがあったりします。

こちらは友人が発表している資料なのですが非常にわかりやすくまた彼もコミッターなので是非一読してみるといいかもしれません。

https://speakerdeck.com/moricho/gvisordeshi-xian-surukorekarafalsekontenasekiyuritei


# 感想
runcが一番企画としてしりたかったこともあり非常に有意義でした！ありがとうございました。
# 反省
夜の時間帯でも自分の部屋を確保してもっと会話量を増やしたい。