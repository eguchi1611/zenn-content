---
title: "最小構成で LaTeX + Dev Container"
emoji: "👻"
type: "tech" # tech: 技術記事 / idea: アイデア
topics: ["devcontainer", "latex", "vscode"]
published: false
---

## LaTeXの環境構築って難しいよね

私は大学に入ってからLaTeXでレポートを書くようになりましたが、もうすでにウンザリです。ネットには情報が散乱していてどれを信じたらいいのかサッパリです。~~この記事を世に放出したらもっと情報が増えるじゃないか？いいえ聞こえません~~

LaTeXのインストールはパソコンに破壊的変更をしかねないので、パソコンを常に綺麗に保っていきたい私にはとても受け入れられるモノではないですね。ベストプラクティスっぽいのが定着したので私のパソコンを犠牲に試行錯誤してきたので役に立てれば幸いです。

## 対象読者

- LaTeXの環境構築にうんざりしてる
- Dev ContainerのLaTeX執筆環境に興味がある

VSCodeのインストール方法、Dockerのインストール方法、VSCodeのインストール方法等は触れません。大学に入って初めてパソコンを触った、LaTeXの環境を準備しないといけないけど、どうしたらいいのか分からない、などという場合には**この記事は向いていません。**

## TL;DR

以下のリポジトリに完成品があります。どうぞご自由に煮るなり焼くなりしてください。

https://github.com/eguchi1611/latex-workspace

## 解説します

GitHubをみて理解できれば良いですが、理解できないとモヤモヤして嫌ですよね。どう動いているのか分からないのにとりあえず動けばいいという考えの人は私とは分かり合えないですね。~~聞いてない~~

この環境は主に2つのファイルから構成されています。Dev Containerの構成に`devcontainer.json`、`Dockerfile`ですね。  
LaTeX Workshopの構成とかに`.latexmkrc`と、`.vscode`ディレクトリ内のが頑張ってくれています。

### Dev Containerの構成ファイル