---
title: "自己紹介"
date: 2020-12-16T01:14:24+09:00
draft: false
---
# Info

## Basic
1995年　神奈川県

## Back born
エンジニアのきっかけは、小学生の時にみたブラッディマンデイをみたことが割と最初な気がします。

当時祖母に当時は8000円ちかくしたハッキングの本をかってもらってからが今の原点かなと思います。

そして物事の仕組みなどを理解するのが今でも好きで仕事においても正しく理解して愚直に実装することが重要だと考えております。

とくに自分が技術で好きな領域がセキュリティ・パフォーマンスチューニング・ネットワーク・Linux Kernel

またアルゴリズムも非常に需要だと考えております

# Picking up the work so far
- 想定負荷5000RPSの参照、100RPSの書き込みがあるサービスの実装とインフラ設計とセキュリティ用件、負荷試験を開発メンバ３人ほどで行いました。実装は読み込みが多めだったのでエッジによるキャッシュをおこい。負荷試験は負荷をかけるのも大変だったのでwrk2を使ったりしました。
- 1000万レコード以上のデーターパイプラインの構築 apaceh beamをつかってストーム基盤の実装とBigqueryによるETL・ELT基盤をdatastoreで構築しました。より高速にbeamSDKを実行するためにavroやgsonなどをとりいれました。
- オンデマンド動画配信において負荷分散と最適サイズの動画変換のAWSを中心に自前の配信基盤とm3u8コンバーターの実装をしました。

# Carrier
## Company
- [株式会社ヤプリ](https://yappli.co.jp/) 2020~    
- [株式会社サイバーエージェント](https://www.cyberagent.co.jp/) 2019~2020
    - [新卒内定者による新子会社　株式会社Cyber Palを設立](https://www.cyberagent.co.jp/news/detail/id=23000)
    - [小規模組織にgke istio導入した結果」後藤　秀昂（株式会社Cyber Pal）](https://cyberagent.ai/blog/pr/culture/5649/)

## intern
- [株式会社AbemaTV](https://abema.tv/) 2018~2019
- [UUUM株式会社](https://www.uuum.co.jp/) 2017~2018
- [deBit株式会社](https://debit.co.jp/) 2017~2018

## University
- 武蔵野大学経済学部卒業 2019年度卒業
- 研究内容 ゲーム理論 マッチング理論
- 卒業論文 検索エンジンの普及と消費者の行動について

# Publish
- [新進気鋭のホワイトハッカーとアンチウイルスソフトがガチンコ対決! 戦いの結末をレポート](https://news.mynavi.jp/kikaku/20180720-665544/)
- [istio-ingressgateway ssl https 証明書 中間証明書 導入するよ](https://qiita.com/hidexir/items/645b6d6cabf239d870d0)
- [Nginxとnodejsで認証プロキシを実現する※basic認証じゃないよ！！](https://qiita.com/hidexir/items/6d2da4e431641cbf0122)
- [GKEにistio導入をした話](https://hidexir.hatenablog.com/)

# Skill
## Lang
- Go
- Rust
- Python
- Java
- Scala
- C++
- TypeScript

## Infra
- AWS
- GCP
- Kubernetes

## editor
vim emacs(日本語書く時)

# My Project

## [ISUCON10](https://isucon.net/archives/55008744.html)
rank #166 top 30% team yagyu

## [x86 emulator](https://github.com/hidexir/x86emu)
x86アーキテクチャの実行環境のエミュレーターをrustでフルスクラッチしました。

## [動画配信サービス](https://wantty.app/)
動画配信サービスです。トレーナ さんやスポーツ選手が動画をアップロードしてストリームとして視聴できます。

## [イーサリアムトークンを用いたサービス](https://www.peace-coin.org)
ソリディティフレームワークを用いて主にサーバーサイドを担当しました。

## [性格診断サービス](https://www.zelfium.com/ja/)
性格判断のパターンがとにかくおおいので一度是非やってみください。ユーザーからの質問の回答いかに高速に分類するかのアルゴリズムと裏でもつデーター構造は結構考えました。
主にツリー構造をもちいて高速化に成功しました。

## [ゾンビゲーム](https://apps.apple.com/jp/app/escape-from-uncle/id1444505240)
サイバーエージェント時代の同期と２人で作成しました。[解説](https://gameappch.com/app/?app=06132)をしているかたまでいて非常にうれしかったです。
自分は主に3Dオブジェクトは購入して中のロジックやmapのレイアウト、カメラの視点コントロールなどの実装をしました。