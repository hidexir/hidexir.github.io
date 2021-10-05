---
title: "自己紹介"
date: 2020-12-16T01:14:24+09:00
draft: false
---
# Info
# Intro
閲覧ありがとうございます。  
ソフトウェアエンジニアです。コンピューターの基礎からアプリケーションまで好きです。  
[FAQ]({{< ref "/blogs/faq.md" >}})もあるのでそちらを見ていただければと思います。

## Basic
- 1995年生まれ

# Carrier
- [株式会社ヤプリ](https://yappli.co.jp/) 2020~    
- [株式会社サイバーエージェント](https://www.cyberagent.co.jp/) 2019~2020
    - [新卒内定者による新子会社　株式会社Cyber Palを設立](https://www.cyberagent.co.jp/news/detail/id=23000)
    - [小規模組織にgke istio導入した結果」後藤　秀昂（株式会社Cyber Pal）](https://cyberagent.ai/blog/pr/culture/5649/)
    - [株式会社AbemaTV](https://abema.tv/) 2018~2019
- [UUUM株式会社](https://www.uuum.co.jp/) 2017~2018
- [deBit株式会社](https://debit.co.jp/) 2017~2018

# Picking up　※内容は技術よりです。
## ライブ配信でテックリード業務
想定負荷5000RPS以上で1:1:Nのライブ配信サービスの開発  
大規模ということもあり、Go言語をバックエンドインフラにKubernetes(GKE)を採用しました。またネットワーク全体の関しにistioを試みました。負荷試験やセキュリティ用件など厳しかったですが、少人数により開発しました。  
もともと配信をm3u8とう動画配信のストリーミングを自作をこころみたのですが、インフラコストの兼ね合いや配信部分は主に外部のSDKを採用したりなど最終的なは内部の重要部分はすべてGoで作成しました。  
Go自体のパフォーマンスチューニングなども行いREADに関しては1coreで1000RPSをクリアしました。また書き込みに関しても100~300RPSの性能をだし、マシンのリソースをおしみなく使いました。  
セキュリティでは主にインフラとバックエンドに関する部分もベンダー含め担当しました。内容としてはburpsuiteを用いて通信の改竄などを起きた際のサービス影響やSQLやCSRF、認証などを攻撃ベースでベンダとのダブルチェックを行いました。  
## データーパイプライン構築
3TB以上を毎日集計し、マルチテナントプラットフォームにのダッシュボード（データーがいろいろみれる管理画面みたいなやつ）を作成しました。  
データー量が大きいので、GCPのデーターフローを採用しました。理由は安くてフルマネだからです。  
また結構内部での変換処理がいろいろあったのでApache beam SDK (java)をもちいて自作テンプレートをかきました。また高速化を図るため、内部のデーターのシリアライズはAvroをつかうことで大幅なデーター削減と高速化を実現しました。  
参考に[メルカリでの事例](https://engineering.mercari.com/blog/entry/mercari-dataflow-template/)や、[オープンソース](https://github.com/mercari/DataflowTemplate)をみました。  
# Back born
もともと小さい頃からコンピューターは好きでした。当時はネットサーフィンがメインで簡単なプログラムの本などで見様見真似でした。  
大学時代にフロントの仕事を受けながらより本格的にバックエンド、インフラをはじめ、自分でサービスをつくったりしたものの事業作りに無知だったため、  
仮想通貨事業でRustでjsonパーサーをつくったり、AbemaTVで広告の開発をしておりました。  
当時は低レイヤーが好きだったこともあり、Googleのエンジニアに漠然となりたいと考えていたのですが、アルゴリズムや英語能力がたりないと感じたので、国内のもっとも力がつくと考えそのままAbemaの開発をするためCyBerAgentに入社しました。  
# Publish
- [新進気鋭のホワイトハッカーとアンチウイルスソフトがガチンコ対決! 戦いの結末をレポート](https://news.mynavi.jp/kikaku/20180720-665544/)
- [istio-ingressgateway ssl https 証明書 中間証明書 導入するよ](https://qiita.com/hidexir/items/645b6d6cabf239d870d0)
- [Nginxとnodejsで認証プロキシを実現する※basic認証じゃないよ！！](https://qiita.com/hidexir/items/6d2da4e431641cbf0122)
- [GKEにistio導入をした話](https://hidexir.hatenablog.com/)

# Skill
一般的にまともに仕事をしているとかなりの量になるので、ここでは中でも好きなこと、得意なことを中心に載せております。
## Cloud 
AWSやGCPサービスを作るにあたってのDBやネットワーク、ストレージ、システムデザインはできます。 またオンプレ（VPS）による開発も行っておりました。
## Lang
Go Rust Python Java Scala C++ TypeScript
## Keywords
Kubernetes Terraform Fastly Nginx Istio Envoy
## editor
vim 好きな方は是非話しましょう。
# Hobby
## [ISUCON10](https://isucon.net/archives/55008744.html)
わりと上位になりました。
rank #166 team yagyu
## ISUCON9
たしか半分くらいだった
## [x86 emulator](https://github.com/hidexir/x86emu)
x86アーキテクチャの実行環境のエミュレーターをrustでフルスクラッチしました。
スクラップ はこちら https://zenn.dev/hidexir/scraps/e110b61cdf1857
## [スポーツ知見シェアサービス](https://wantty.app/)
動画配信サービスです。トレーナ さんやスポーツ選手が動画をアップロードしてストリームとして視聴できます。主に動画配信周りとインフラ
## イーサリアムトークンを用いたサービス
趣味で、ソリディティフレームワークを用いて主にサーバーサイドを担当しました。
## [性格診断サービス](https://www.zelfium.com/ja/)
性格判断のパターンがとにかくおおいので一度是非やってみください。ユーザーからの質問の回答いかに高速に分類するかのアルゴリズムと裏でもつデーター構造は結構考えました。
主にツリー構造をもちいて高速化に成功しました。
## [ゾンビゲーム](https://apps.apple.com/jp/app/escape-from-uncle/id1444505240)
サイバーエージェント時代の同期と２人で作成しました。[解説ブログが書かれてた！](https://gameappch.com/app/?app=06132)をしているかたまでいて非常にうれしかったです。
自分は主に3Dオブジェクトは購入して中のロジックやmapのレイアウト、カメラの視点コントロールなどの実装をしました。
