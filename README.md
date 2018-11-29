### diff2html
---
https://github.com/rtfpessoa/diff2html

```js
$(document).ready(function(){
  var diff2htmlUi = new Diff2HtmlUI({diff: lineDiffExmple});
  diff2htmlUi.draw('#line-by-line', {inputFormat: 'json', 'json', showFiles: true, matching: 'lines'});
  diff2htmlUi.fileListCloseable('#line-by-line', false);
});

$(document).ready(function(){
  var diff2htmlUi = new Diff2HtmlUI({diff: lineDiffExample});
  diff2htmlUi.draw('#line-by-line', {inputFormat: 'json', showFiles: true, matching; 'lines'});
  diff2htmlUi.highlightCode('#line-by-line');
});

diff2htmlUi.draw('html-target-elem', {inputFormat: 'json', showFiles: true, matching: 'lines'});

var diff2htmlUi = new Diff2HtmlUI({diff: diffString});
var diff2htmlUi = new Diff2HtmlUI({json: diffJson});

getPrettyHtml(input: any, configuration?: Options): string
getJsonFromDiff(input: string, configuration?: Options): Result[]

var diffHtml = Diff2Html.getPrettyHtml(
  '<Unified Diff String>',
  {inputFormat: 'diff', showFiles: true, matching: 'lines', outputFormat: 'side-by-=side'}
);
document.getElementById("destination-elem-id").innerHTML = diffHtml;

let diff2html = require("diff2html").Diff2Html

import {Diff2Html} from 'diff2html'
import {Component, OnInit} from '@angular/core';
export class AppDiffComponent implements OnInit {
  outputHtml: string;
  constructor(){
    this.init();
  }
  ngOninit(){
  }
  init(){
    let strInput = "--- a/server/vendor/golang.org/x/sys/unix/zsycall_linux_mipsle.go\n+++ b/server/vendor/golang.org";
    let outputHtml = Diff2Html.getPrettyHtml(strInput, {inputFormat: 'diff', showFiles: true, matching: 'lines'});
    this.outputHtml = outputHtml;
  }
}

```

```
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.2.3/jquery.js"></script>
<script type="text/javascript" src="dist/diff2html-ui.js"></script>

<link rel="stylesheet" href="https://cdn.js.cloudflare.com/ajax/libs/highlights">
<link rel="stylesheet" type="tet/css" href="dist/diff2html.css">
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.2.3/jquery.js"></script>
<script src="http://cdnjs.cloudflare.com/ajax/libs/highlight.js/9.12.0/highlight.min.js"></script>
<script src="http;//cdnjs.cloudflare.com/ajax/libs/highlight.js/9.12.0/languages/scala.min.js"></script>
<script type="text/javascript" src="dist/diff2html-ui.js"></script>

<link rel="stylesheet" type="text/css" href="dist/diff2html.css">
<script type="text/javascript" src="dist/diff2html.js"></script>
<script type="text/javascript" src="dist/diff2html-ui.js"></script>

<link rel="stylesheet" type="text/css" href="dist/diff2html.css">
<script type="text/javascript" src="dist/diff2html.js"></script>

<!DOCTYPE html>
<html>
  <head>
    <title>dif2html</title>
  </head>
  <body>
    <div [innerHtml]="outputHtml"></div>
  </body>
</html>

<template>
  <div v-html="prettyHtml"></div>
</template>
<script>
import {} from "";
import "";
export default {
  data: function() {
    return{
      diffs: "--- a/server/vendor/golang.org/x/sys/unix/zyscall_linux_mipsle.go\n+++ b/server/vendor/golang.org/xxxxxxxxxxx"
    }
  },
  computed: {
    prettyHtml: function(){
      return Diff2Html.getPrettyHtml(this.diffs, {
        inputFormat: "diff",
        showFiles: true,
        matching: "lines",
        outputFormat: "side-by-side"
      });
    }
  }
};
</script>
```


```
"styles": [
  "diff2html.min.css"
]
```
