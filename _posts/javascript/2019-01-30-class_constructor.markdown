---
layout: post
title:  "class & constructor"
date:   2019-01-30 19:47:31 +0530
categories: ["javascript"]
author: "Bestests"
---
<link rel="stylesheet" href="/js/highlight/styles/monokai.css" />
<script src="/js/highlight/highlight.pack.js"></script>
<script>hljs.initHighlightingOnLoad();</script>

<h2>Javascript</h2>
<h3>class & constructor</h3>
<pre>
  <code class="javascript">
     class Test {
        constructor (name) {
            this.name = name;
        }
        
        get getName () {
            return this.name;
        }
        
        set setName (name) {
            this.name = name;
        }
     }
     
     const test = new Test("Bestests");
     console.log(test.getName);
     // "Bestests"
     test.setName = "bestests";
     console.log(test.getName);
     // "bestests"
  </code>
</pre>
