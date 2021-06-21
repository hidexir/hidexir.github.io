---
title: "Cloud Native 読書会第6回 ArgoCD"
date: 2021-04-21T20:00:00+09:00
draft: false
---
# はじめに
なおBlogs自分の日常のメモになります。

こんにちは以前にwantedlyの大坪さんの紹介で参加しました。

こちらから当日の内容は見ることができます。

https://zenn.dev/potsbo/scraps/8f64a637cf50f5

# 本文
もともとクラウドネイティブ技術がすきでArgoCDもArgoWorkflowも業務で使ったいたのですが、内部の仕組みまで深ぼることがなかなか機会として少なかったこともありました。

時間はそこまで長くはないのですが、Goで実装がされており、main関数のエントリーポイントをベースに実装を読み進めました。

参加しているメンバーもやはりSREが業務の中心になっているかたや、もともと内部実装にある程度詳しいかたもいたのですが、Goを読むということは変わりなく。非常によかったです。

サービスの可用性を図る際にHeathCheckを行うと思うのですが、Argocdには状態が複数ありドキュメントでも多くは語られていないケースはあるのですが、Argoの場合だといかにあります。

HealthStatusCode の定義

https://github.com/argoproj/gitops-engine/blob/master/pkg/health/health.go#L8-L26

```Go
// Represents resource health statusAlexander Matyushentsev, 11 months ago: • docs: document 'top level' packages (#44)
type HealthStatusCode string


const (
	// Indicates that health assessment failed and actual health status is unknown
	HealthStatusUnknown HealthStatusCode = "Unknown"
	// Progressing health status means that resource is not healthy but still have a chance to reach healthy state
	HealthStatusProgressing HealthStatusCode = "Progressing"
	// Resource is 100% healthy
	HealthStatusHealthy HealthStatusCode = "Healthy"
	// Assigned to resources that are suspended or paused. The typical example is a
	// [suspended](https://kubernetes.io/docs/tasks/job/automated-tasks-with-cron-jobs/#suspend) CronJob.
	HealthStatusSuspended HealthStatusCode = "Suspended"
	// Degrade status is used if resource status indicates failure or resource could not reach healthy state
	// within some timeout.
	HealthStatusDegraded HealthStatusCode = "Degraded"
	// Indicates that resource is missing in the cluster.
	HealthStatusMissing HealthStatusCode = "Missing"
)
```

つまり、ソースコードリーティングをしないとわからないこともあるのがクラウドネイティブの現状です。

そしてコンテナ技術が中心となるなかKubernetesはデファクトスタンダードになりつつあるなか、CRMの理解をする上でもここらへんのベース理解は今後も重要になりそうです。

# 感想・反省
全体がなんとなく理解できてよかった。

実装を読むのはシンプルに楽しい細かいオプションや小さいことにきづけたのはよかった。

やはりプロジェクト自体が大きな理解だったので時間あるときに細かい部分おってみたい。

自分もvim tmuxなので、久しぶりに人のあまり他の人の開発環境見る機会がないのでよかった