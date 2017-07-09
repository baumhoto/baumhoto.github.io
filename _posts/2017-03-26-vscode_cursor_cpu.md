---
layout: post
title: "VSCode wasting CPU resources on blinking cursor"
date: 2017-03-26 10:15:00
tags: vscode chrome bug
description: VsCode bug
excerpt_separator: <!--more-->
comments: true
fixed: false
---

Recently some reports came up that [Visual Studio Code](https://code.visualstudio.com) was wasting CPU resources to render a blinking cursor [GitHub Issue](https://github.com/Microsoft/vscode/issues/22900).

Turned out that it is actually a bug in Chrome that needs to be fixed [Chrome Bug Ticket](https://bugs.chromium.org/p/chromium/issues/detail?id=361587). As the chrome fix might be still some time off the best thing to do right now is to add the following line to your VsCode config:

{% highlight json %}
 "editor.cursorBlinking": "solid"
{% endhighlight json %}

<!--more-->

VSCode is a currently my prefered code-editor (next to vim which i use for quick edits on the terminal), so i disabled the blinking cursor.

If you wonder how VSCode relates to Chrome it's because VsCode (like Atom) is build on Electron (which is a combination of Chromium and NodeJs) to write client applications with NodeJs/Javascript. Electron was created by Github to create Atom and Microsoft used Electron to build VS Code.

So MS has build a piece of software based on a google product. It's a strange world we live in nowadays, but i like it:)