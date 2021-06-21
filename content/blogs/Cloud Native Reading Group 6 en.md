---
title: "Cloud Native Reading Group #6: ArgoCD"
date: 2021-04-21T20:00:00+09:00
draft: false
---
# Introduction
This is a blog about my daily life.

Hello, I joined this event through the introduction of Mr. Ohtsubo from wantedly.

You can see the content of the day here.

https://zenn.dev/potsbo/scraps/8f64a637cf50f5

# Text
I've always loved cloud-native technologies, and I've used ArgoCD and ArgoWorkflow in my work, but I haven't had many opportunities to dive deep into the inner workings of them.

It was not that long, but it was implemented in Go, and we read through the implementation based on the entry point of the main function.

Some of the participants were also SREs, and some of them were familiar with the internal implementation, but they were still reading Go. It was very good.

In Argocd, there are multiple health statuses, and there are cases where the documentation doesn't say much about them, but in Argo, there are many.

HealthStatusCode definition

https://github.com/argoproj/gitops-engine/blob/master/pkg/health/health.go#L8-L26

```Go
// Represents resource health statusAlexander Matyushentsev, 11 months ago: - docs: document 'top level' packages (#44)
type HealthStatusCode string


const (
	// Indicates that health assessment failed and actual health status is unknown
	HealthStatusUnknown HealthStatusCode = "Unknown"
	// Progressing health status means that the resource is not healthy but still has a chance to reach a healthy state
	HealthStatusProgressing HealthStatusCode = "Progressing"
	// Resource is 100% healthy
	HealthStatusHealthy HealthStatusCode = "Healthy"
	// Assigned to resources that are suspended or paused. The typical example is a
	// [suspended](https://kubernetes.io/docs/tasks/job/automated-tasks-with-cron-jobs/#suspend) CronJob.
	HealthStatusSuspended HealthStatusCode = "Suspended"
	The typical example is a // [suspended]() CronJob. HealthStatusSuspended HealthStatusCode = "Suspended" // Degrade status is used if resource status indicates failure or resource could not reach healthy state
	// within some timeout.
	HealthStatusDegraded HealthStatusCode = "Degraded"
	// Indicates that resource is missing in the cluster.
	HealthStatusMissing HealthStatusCode = "Missing" // Indicates that resource is missing in the cluster.
)
````

In other words, there are some things that are cloud-native that you can't understand without source code letting.

And with container technology taking center stage and Kubernetes becoming the de facto standard, it will be important to understand the base of CRM in the future.

# Impressions and reflections
I'm glad I could understand the whole thing somewhat.

Reading the implementation was simple and fun, and it was good to notice the small details and options.

I'd like to try to understand the details when I have time.

I'm also a vim tmux user, so it's been a while since I've had a chance to see someone else's development environment. Translated with www.DeepL.com/Translator (free version)