

わからなかったら飛ばして脳死でコマンド打ってもOK
-------------------------

フロントエンド編(環境構築)
==============

やること
-  nodeをインストール
-  vue-cliをインストール
-  vueを立ち上げて動作させてみる



Step1 環境構築
----------

めんどくさいですが環境構築から始めましょう

まずはnodenv

[https://qiita.com/1000ch/items/41ea7caffe8c42c5211c](https://qiita.com/1000ch/items/41ea7caffe8c42c5211c)
[https://qiita.com/1000ch/items/41ea7caffe8c42c5211c](https://qiita.com/1000ch/items/41ea7caffe8c42c5211c)

nodevnをダウンロードして動かせるようにすると

npm(node package manger)が使用できるようになっていると思います。

Nodeって何？
--------

> V8 is Google’s open source high-performance JavaScript and WebAssembly engine, written in C++. It is used in Chrome and in Node.js, among others. It implements ECMAScript and WebAssembly, and runs on Windows 7 or later, macOS 10.12+, and Linux systems that use x64, IA-32, ARM, or MIPS processors. V8 can run standalone, or can be embedded into any C++ application.

[](https://v8.dev/)[https://v8.dev/](https://v8.dev/)

> サーバーサイドの JavaScript 実行環境。

> Google V8 JavaScript エンジンを使用しており、高速。

> Linux サーバにインストールして使用することが多いが、macOS 版や、Windows 版もある。

> npm (Node Package Manager) と呼ばれるパッケージ管理システムを同梱。

> ノンブロッキングI/O と イベントループ アーキテクチャにより、10K問題 (クライアント1万台レベルになると性能が極端に悪化する問題) に対応。

[](http://www.tohoho-web.com/ex/nodejs.html)[http://www.tohoho-web.com/ex/nodejs.html](http://www.tohoho-web.com/ex/nodejs.html)

とほほNode.js入門

ブラウザ上でしか動作しなかったJavascriptをlinux, Mac, Windows上でも動作するようにしたもの。

NPM(Node Package Manager)
-------------------------

npm公式サイト about npm

[](https://docs.npmjs.com/about-npm)[https://docs.npmjs.com/about-npm](https://docs.npmjs.com/about-npm)

今回使用するのはパッケージ管理の部分なので使用するのは以下のコマンド

npm install

概要は以下(飛ばし読みでもok)

```
npm install (with no args, in package dir)
npm install [<@scope>/]<name>
npm install [<@scope>/]<name>@<tag>
npm install [<@scope>/]<name>@<version>
npm install [<@scope>/]<name>@<version range>
npm install <alias>@npm:<name>
npm install <git-host>:<git-user>/<repo-name>
npm install <git repo url>
npm install <tarball file>
npm install <tarball url>
npm install <folder>
aliases: npm i, npm add
```

[](https://docs.npmjs.com/cli/v7/commands/npm-install)[https://docs.npmjs.com/cli/v7/commands/npm-install](https://docs.npmjs.com/cli/v7/commands/npm-install)


Vueを導入する
---
Why Vue

日本での使用率はReactと争っている。

国内での採用事例が多いい

```bash
npm install -g @vue/cli
```


```
vue create my-project
```

question1
❯ Manually select features

question2
![[sec1_1.png]]

question3
- 3.x
(どちらでもいい)

これ以降の質問はすべてEnterを押すと、Vueの環境がmy-project/以下に自動で立ち上がる。




```
cd my-project
npm run serve
```

ブラウザで `http://localhost:8080/` をアクセスするとサンプルが表示される。
![[sec1_2.png]]


参考サイト
https://jp.vuejs.org/v2/guide/installation.html
https://qiita.com/567000/items/dde495d6a8ad1c25fa43
