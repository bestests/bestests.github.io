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
<input type="text" id="inputObj" />
<div id="resultObj"></div>
<pre>
  <code class="javascript">
      // input object &lt;input type="text" id="inputObj" /&gt;
      // reulst obejct &lt;div id="resultObj"&gt;&lt;/div&gt;
      const inputObj  = document.getElementById("inputObj");
      const resultObj = document.getElementById("resultObj");
      
      let timer;
      
      const inputListener = function (event) {
          if(timer) clearTimeout(timer);
          timer = setTimeout(() => {
              // Do something!!
              console.log(this.value);
              resultObj.innerText = this.value;
          }, 250);
      }
      
      inputObj.oninput = inputListener.bind(inputObj);
  </code>
</pre>
