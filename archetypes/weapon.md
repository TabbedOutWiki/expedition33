---
translationKey: {{ lower .File.ContentBaseName }}
title: {{ replace .File.ContentBaseName `-` ` ` | title }}
description: "{{ replace .File.ContentBaseName `-` ` ` | title }} is a weapon in Clair Obscur: Expedition 33 equipable by {{ .Site.Params.character | title }}{{ if .Site.Params.character2 }} and {{ .Site.Params.character2 | title }}{{ end }}. It uses {{ .Site.Params.element | title }} attacks that scale in power with the {{ .Site.Params.primary_attribute | title }}{{ if .Site.Params.secondary_attribute }} and {{ .Site.Params.secondary_attribute | title }} attributes{{ else }} attribute{{ end }}."

element: {{ .Site.Params.element | lower }}
attributes:
  primary: {{ .Site.Params.primary_attribute | lower }}
  {{ if .Site.Params.secondary_attribute }}secondary: {{ .Site.Params.secondary_attribute | lower }}{{ end }}
passives:
  - ""
  - ""
  - ""
multiplier: {{ .Site.Params.multiplier }}

categories:
tags:
---

{{< infobox-weapon >}}

**{{ replace .File.ContentBaseName `-` ` ` | title }}** is a weapon equipable by [{{ .Site.Params.character | title }}](/character/{{ .Site.Params.character | lower }}){{ if .Site.Params.character2 }} and [{{ .Site.Params.character2 | title }}](/character/{{ .Site.Params.character2 | lower }}){{ end }}.

## Acquisition

## Strategy

## Upgrades

{{< weapon-upgrade-table >}}

## Trivia

## Related articles
