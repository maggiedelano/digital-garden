---
title: Using Custom JS in Roam
---

Assuming you already have the code you need to paste into your graph, this note will show you how to get the custom javascript itself to run in your [[Roam Research]] graph.

1. Create a {% raw %}`{{[[roam/js]]}}`{% endraw %}  block anywhere in your graph. I usually like to put them either on the `[[roam/js]]` page or on the page for the name of the feature or plugin.
2. Create a block *below* the {% raw %}`{{[[roam/js]]}}`{% endraw %} block you just created. Type tab so that this new block is nested *under* the {% raw %}`{{[[roam/js]]}}`{% endraw %} block.
3. Inside this new block, type three backticks (\`\`\`) in a row. Roam should autocomplete with a matching set of backticks and then create a javascript code block (if it doesn't, try hitting escape). You can also create a javascript code block by typing `/javascript code block` and selecting it from the drop down menu. 
5. Paste the code into the javascript code block.

If you've done everything correctly, this is what your setup should look like:

<img src="/garden/assets/roamjsblock.png"/>

**Important Note:** You run javascript in Roam at your own risk; be sure you trust the source. Further reading: [security in Roam Research](https://www.zsolt.blog/2021/03/roam-sex-ed.html).

