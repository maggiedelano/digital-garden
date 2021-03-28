---
title: Using Custom JS in Roam
---

Assuming you already have the code you need to paste into your graph, this note will show you how to get the custom javascript itself to run in your [[Roam Research]] graph.

1. Create a `{{[[roam/js]]}}` block anywhere in your graph. I usually like to put them either on the [[roam/js]] page or on the page for the name of the feature or plugin.
2. Create a block *below* the `{{[[roam/js]]}}` you just created. Type tab so that this new block is *under* the other graph.
3. Type three backticks (\`\`\`) in a row. Roam will autocomplete with a matching set of backticks.
4. Hit escape; you should now have a javascript code block.
5. Paste the code into the javascript code block.

<img src="/garden/assets/roamjsblock.png"/>

You run javascript in Roam at your own risk; be sure you trust the source. Further reading: [security in Roam Research](https://www.zsolt.blog/2021/03/roam-sex-ed.html).