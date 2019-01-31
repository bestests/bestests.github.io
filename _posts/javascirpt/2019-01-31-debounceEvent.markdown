---
layout: post
title:  "Debounce Event"
date:   2019-01-31 23:43:00 +0530
categories: ["javascript"]
author: "Bestests"
---
<link rel="stylesheet" href="/js/highlight/styles/monokai.css" />
<script src="/js/highlight/highlight.pack.js"></script>
<script>hljs.initHighlightingOnLoad();</script>

<h2>Javascript</h2>
<h3>Debounce Event</h3>
<hr />
<pre>
  <code class="javascript">
      // input object "<input type="text" id="inputObj" />"
      const inputObj = document.getElementById("inputObj");
      
      let timer;
      
      const inputListener = function (event) {
          if(timer) clearTimeout(timer);
          timer = setTimeout(() => {
              // to do
              console.log(this.value);
          }, 250);
      }
      
      inputObj.oninput = inputListener.bind(inputObj);
  </code>
</pre>
