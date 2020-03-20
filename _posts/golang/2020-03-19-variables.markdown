---
layout: post
title:  "Variables"
date:   2020-03-19 09:38:00 +0530
categories: ["golang"]
author: "Bestests"
---
<link rel="stylesheet" href="/js/highlight/styles/monokai.css" />
<script src="/js/highlight/highlight.pack.js"></script>
<script>hljs.initHighlightingOnLoad();</script>

<h1>#Variables</h1>
---
<pre>
  <code class="go">
      // 타입 생략 가능(생략 시 초기 데이터로 타입 정해짐)
      var test1 = "test1"
      const test2 = "test2"
      
      // 타입 명시 가능
      var test3 string = "test3"
      const test4 string = "test4"
      
      func test () {
         // 함수안에서만 가능
         test5 := "test5"
      }
  </code>
</pre>
---
