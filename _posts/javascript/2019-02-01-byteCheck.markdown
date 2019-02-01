---
layout: post
title:  "Byte Check"
date:   2019-02-01 19:46:00 +0530
categories: ["javascript"]
author: "Bestests"
---
<link rel="stylesheet" href="/js/highlight/styles/monokai.css" />
<script src="/js/highlight/highlight.pack.js"></script>
<script>hljs.initHighlightingOnLoad();</script>

<h2>Javascript</h2>
<h3>Byte Check Function</h3>
<input type="text" id="inputObj" />
<button type="button" id="btnObj">button</button>
<div id="resultObj" style="border: 1px solid black;"></div>
<pre>
  <code class="javascript">
      const inputObj  = document.getElementById("inputObj");
      const btnObj    = document.getElementById("btnObj");
      const resultObj = document.getElementById("resultObj");
      
      const btnOnclickListener = function (event) {
          resultObj.innerText = this.value;
      };
      
      btnObj.onclick = btnOnclickListener.bind(inputObj);
  </code>
</pre>

<script>
      const inputObj  = document.getElementById("inputObj");
      const btnObj    = document.getElementById("btnObj");
      const resultObj = document.getElementById("resultObj");
      
      const btnOnclickListener = function (event) {
          resultObj.innerText = this.value;
      };
      
      btnObj.onclick = btnOnclickListener.bind(inputObj);
</script>
