---
layout: default
---

# flowchart.js

_Code:_

<!-- markdownlint-disable MD031 -->

```;
`​``flowchart
st=>start: Start:>
e=>end:>
op1=>operation: My Operation
sub1=>subroutine: My Subroutine
cond=>condition: Yes or No?:>
io=>inputoutput: catch something...
para=>parallel: parallel tasks

st->op1->cond
cond(yes)->io->e
cond(no)->para
para(path1, bottom)->sub1(right)->op1
para(path2, top)->op1
`​``
```

<!--
There's a Zero Width Space between two of the inner closing three backticks
to prevent them from being interpreted as closing the outer opening three
backticks.
-->

<!-- markdownlint-enable MD013 -->

_Result:_

![flowchart.js example](/assets/img/flowchart.png)

(Source: [flowchart.js.org](http://flowchart.js.org))
