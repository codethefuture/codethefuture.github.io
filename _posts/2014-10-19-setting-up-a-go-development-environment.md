---
layout: post
title: "Go言語の設定とIntelliJ IDEAの設定"
description: ""
category: development
tags: [IntelliJ IDEA, go]
---
{% include JB/setup %}

### GolangをHomebrewでインストール

Homebrewでインストールできるので楽ですね。

```Terminal
brew update
brew install go
```
### 次に環境変数を設定

```zsh:.zshrc
export GOROOT=/usr/local/opt/go/libexec
export GOPATH=$HOME/.go
```

### Mac OS Xの場合は以下の設定が必要

https://github.com/go-lang-plugin-org/go-lang-idea-plugin/blob/master/Missing%20ENV.md#--mac-os-x

```launchd.conf
setenv GOROOT /usr/local/opt/go/libexec
setenv GOPATH $HOME/.go
```

### 設定を反映する

```Terminal
source ~/.zshrc
launchctl < /etc/launchd.conf
```

#### 設定を確かめる
```Terminal
echo $GOROOT;echo $GOPATH
```

### Intellij IDEA setting

まずはプラグインをインストール

1.Quick Start
2.Plugins
3.[Go language support plugin](https://github.com/go-lang-plugin-org/go-lang-idea-plugin)をインストール

次にGolangのSDKの設定

1.Quick Start
2. Configure
3. Project Defaults
4. Project Structure
5. Project SDK - New button
6. Go SDK
7. Pathを指定する
  - /usr/local/Cellar/go/1.3.1/libexec

